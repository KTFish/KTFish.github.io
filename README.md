# personal website development repo

## Deployment

Deployments to [KTFish.github.io](https://ktfish.github.io) are triggered manually from `main` via the **Deploy to KTFish.github.io** GitHub Action.

### Steps
1. Tag the release commit on `main`:
   ```sh
   git checkout main
   git tag v1.0.0 && git push origin v1.0.0
   ```
2. In GitHub Actions, select **Deploy to KTFish.github.io** → **Run workflow** on `main`.

*(Note: Requires a `DEPLOY_PAT` secret with write access to `KTFish/KTFish.github.io`. You can also supply `release_tag` directly in the workflow dispatch input.)*

