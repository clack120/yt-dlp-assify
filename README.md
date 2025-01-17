## Installation

Requires `yt-dlp` version `2025.01.15` or above, and [YTSubConverter](https://github.com/arcusmaximus/YTSubConverter/releases/latest).

You can install this package with:
```
pip install -U https://github.com/yt-dlp/yt-dlp-sample-plugins/archive/master.zip yt-dlp
```
You should use yt-dlp from pip, not executable from releases page.  
Ensure that [`YTSubConverter`](https://github.com/arcusmaximus/YTSubConverter/releases/latest) is in your PATH. Might require `mono` if you are using Linux.
###### You can install AUR Package if you are using archlinux. `yay -Sy ytsubconverter-git`, then link `ytsubconverter-git` to `YTSubConverter` inside binary folder.

---

## Usage

To use it, simply run:

```
yt-dlp --embed-subs --postprocessor-args assify $YOUTUBE_VIDEO_URL
```
##### Example: `yt-dlp -fba+bv --extractor-args youtube:skip=translated_subs --embed-subs --sub-lang=all,-live_chat --sub-format=srv3/ytt --use-postprocessor assify --embed-thumbnail --embed-metadata https://www.youtube.com/watch?v=8MImc3MxYZg`
##### Note: output format must be .mkv without `--merge-(whatever)=mkv` because it won't fix error (at least on my environment; idk why)

---

## Contributing

Pull requests and issues are super welcome! Feel free to submit any bug reports or feature suggestions.
###### Actually, I will never update this repository until someone makes pull request, probably.

---

## License

This project is licensed under the Unlicense, same as the [yt-dlp](https://github.com/yt-dlp/yt-dlp) does. See the [LICENSE](LICENSE) file for details.
