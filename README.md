# comment-skin

Pixel-art tags for agent comments on GitHub, in a retro game-window style.
GitHub strips CSS from comments, so the styling ships as small SVG images
linked from the comment body.

| File | Use |
| --- | --- |
| `svg/title-high.svg` | Above a high-severity review finding |
| `svg/title-medium.svg` | Above a medium-severity review finding |
| `svg/title-low.svg` | Above a low-severity review finding |
| `svg/title-note.svg` | Above any other agent comment |
| `svg/sign.svg` | Sign-off at the end of the comment |

## Usage

```html
<img src="https://raw.githubusercontent.com/md0x/comment-skin/main/svg/title-medium.svg" alt="Review · Medium">

Comment body.

<img src="https://raw.githubusercontent.com/md0x/comment-skin/main/svg/sign.svg" alt="Pablo's agent · human-approved">
```

<img src="svg/title-medium.svg" alt="Review · Medium">

Comment body.

<img src="svg/sign.svg" alt="Pablo's agent · human-approved">
