# SECOND-Grasp Visualizations

This repository contains a static GitHub Pages site for supplementary videos.

## Folder structure

```text
SECOND-Grasp-Visualizations/
├── index.html
└── videos/
    ├── overview.mp4
    ├── semantic_grasp_01.mp4
    ├── semantic_grasp_02.mp4
    ├── semantic_grasp_03.mp4
    ├── semantic_grasp_04.mp4
    ├── unseen_object_01.mp4
    ├── unseen_object_02.mp4
    ├── full_method.mp4
    └── ablation.mp4
```

## Usage

1. Rename your videos to match the filenames above, or edit the paths in `index.html`.
2. Upload `index.html` and the `videos/` folder to the repository.
3. In GitHub, open **Settings → Pages**.
4. Set **Source** to `Deploy from a branch`.
5. Select `main` and `/(root)`, then save.

The site URL will be:

```text
https://anonymousproject-lab.github.io/SECOND-Grasp-Visualizations/
```

## Recommended video encoding

```bash
ffmpeg -i input.mp4   -c:v libx264   -crf 25   -preset medium   -pix_fmt yuv420p   -movflags +faststart   -an   output.mp4
```

Keep each file below GitHub's per-file upload limit.
