# Development Workflow

## Branch Strategy

- **`master`** → Live production website at davidsorge.net
- **`development`** → Ongoing development work
- **Feature branches** → Specific features or content additions

## Workflow

### For Development Work
1. Work on the `development` branch (current)
2. Create feature branches for specific additions:
   ```bash
   git checkout -b feature/new-research-project
   git checkout -b feature/update-teaching-content
   git checkout -b feature/site-improvements
   ```

### Publishing Changes
1. When ready to publish, merge to `master`:
   ```bash
   git checkout master
   git merge development
   git push origin master
   ```
2. GitHub Actions will automatically deploy to davidsorge.net

### Development Guidelines
- Keep incomplete/draft content on `development` or feature branches
- Only merge to `master` when content is ready for public viewing
- Test locally before merging to `master`

## Current Status
- **Live Site:** Content as of October 1, 2025
- **Development:** Ready for new additions and improvements