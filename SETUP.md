# Upload and activation guide

1. On GitHub, create the public profile repository `yogesba/yogesba` (its name must exactly match the account username) or open your existing repository.
2. Upload **README.md**, the complete **assets/** folder, and **.github/workflows/snake.yml** to the root. Uploading only README.md will break the local animations.
3. Commit changes to the repository default branch. The banner, hand, radar, response cycle and terminal GIFs will appear immediately after GitHub renders the README.
4. In **Settings > Actions > General**, enable the actions and permit GitHub Actions to write to the repository, if your repository settings require it. `snake.yml` already requests `contents: write`.
5. On the **Actions** tab, open **Generate contribution snake** and select **Run workflow**. It publishes generated SVG assets to an `output` branch. It also runs once per day.
6. Refresh your GitHub profile after that workflow succeeds to view the contribution snake.

## Known constraints
- GitHub READMEs strip most custom inline CSS and JavaScript. Animations therefore use self-contained GIF files and remote animated SVG providers.
- GitHub streak, activity graph, visitor count and typing SVG are hosted by third parties. If a service is down or blocked, that widget may not appear. All custom GIFs remain in your repository.
- The contribution snake only appears after a successful Actions workflow publishes the `output` branch.
- Animated GIFs may be static for users who enable reduced-motion settings. Keep descriptive alt text.
- Changes to experience, certifications, locations, tools or current projects should be reviewed for accuracy before publication.
- No confidential client diagrams or configurations are included.

## Contents
- `README.md`: complete profile
- `assets/cyber-banner.gif`: animated cybersecurity title banner
- `assets/waving-hand.gif`: waving greeting
- `assets/soc-radar.gif`: scanning radar display
- `assets/response-pipeline.gif`: animated SOC lifecycle
- `assets/security-terminal.gif`: terminal-like security status typing
- `.github/workflows/snake.yml`: automated contribution snake
