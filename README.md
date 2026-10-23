# Pacto PR Assets

Images and other visual assets for Pacto pull requests. Use this repository to host screenshots, GIFs, and feature demos that can be embedded in PR descriptions and review comments.

## Add an asset

1. Create a folder under `assets/` named for the source repository and PR number, such as `assets/pacto/pr-123/`. If the PR is not open yet, use a descriptive feature name instead.
2. Add the image or demo with a descriptive filename, such as `settings-panel.png` or `invite-flow.gif`.
3. Commit and push the asset to `main`, or use GitHub's **Add file → Upload files** action.
4. Open the uploaded file on GitHub and copy its raw file URL.
5. Embed the URL in the PR description or comment:

```markdown
![Settings panel showing the new notification controls](https://raw.githubusercontent.com/covenant-gov/pacto-pr-assets/main/assets/pacto/pr-123/settings-panel.png)
```

The path above is an example; replace it with the URL of an uploaded asset. The `assets/` directory is created when the first asset is added.

## Asset guidelines

- Use lowercase, hyphen-separated folder and file names.
- Prefer PNG or WebP for screenshots and GIF for short animated demos. Compress files while keeping text readable.
- Write alt text that describes the feature or behavior shown.
- Remove credentials, tokens, personal information, and confidential data before uploading. Anyone with repository access can view the files.
- Keep referenced files in place after a PR is merged or closed. Renaming or deleting them can break images in old PRs.
- Use a new filename for an updated screenshot. For a link pinned to an exact version, replace `main` in the raw URL with the asset's full commit SHA.

This repository stores PR assets, not application source code or build artifacts.
