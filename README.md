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
| `svg/title-fixed.svg` | Above a reply saying a review comment was fixed |
| `svg/sign.svg` | Sign-off for comments a human approved before posting |
| `svg/sign-auto.svg` | Sign-off for comments an agent posted on its own |

## Usage

```html
<img src="https://raw.githubusercontent.com/md0x/comment-skin/main/svg/title-medium.svg" alt="Review · Medium">

Comment body.

<img src="https://raw.githubusercontent.com/md0x/comment-skin/main/svg/sign.svg" alt="Pablo's agent · human-approved">
```

Agent-posted comments can name the harness and model after the sign-off.
`align="absmiddle"` keeps the text centred on the tag (GitHub strips `style`):

```html
<img src="https://raw.githubusercontent.com/md0x/comment-skin/main/svg/sign-auto.svg" alt="Pablo's agent · auto-posted" align="absmiddle"> <small>Codex · gpt-5.2</small>
```

<img src="svg/title-medium.svg" alt="Review · Medium">

Comment body.

<img src="svg/sign.svg" alt="Pablo's agent · human-approved">
