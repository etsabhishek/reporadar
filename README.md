# RepoRadar

**See the signal in any repository.** RepoRadar is a lightweight, client-side analyzer for public GitHub repositories. It summarizes public project metadata to help developers decide what to investigate before adopting or contributing to a project.

**Live demo:** https://reporadar-github.vercel.app

## Features

- Search by GitHub URL or `owner/repo`
- Stars, forks, open issues and latest commit activity
- License and repository metadata
- Programming language breakdown
- README preview
- Transparent heuristic score based on activity, documentation, licensing, community signals and repository description
- Responsive dark UI with example repositories
- No account, API key, backend or build step required

## Run locally

This is a static website. Open `index.html` in a browser, or serve the directory with any static file server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Data and limitations

RepoRadar reads public repository data from the GitHub REST API directly in your browser. Requests are subject to GitHub's unauthenticated API rate limits. The number of open issues reflects the first page of results (up to 100), not necessarily every issue in very large repositories. A health score is a transparent heuristic—not a security audit, code-quality assessment, endorsement, or guarantee of project maintenance. A missing license means reuse terms may be unclear; consult the repository and its maintainers.

## Deploy

The site is deployed on Vercel and connected to this GitHub repository for automatic deployments from the `main` branch. No environment variables are required.

## License

No license is specified yet. Add a license before inviting others to reuse or redistribute this project.
