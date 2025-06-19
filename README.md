# GitHub API Test - Colab

This project uses Python and Google Colab to interact with the GitHub public API. It allows users to:

- Search public repositories by keyword
- View recent commits from a selected repository
- List files and folders within a repository
- Handle API rate limits and basic error cases

---

## Requirements

- A GitHub Personal Access Token with the `public_repo` scope
- Python 3 with the following libraries:
  - `requests`
  - `pandas`

---

## How to Use

1. Open the notebook in Google Colab
2. Paste your GitHub token when prompted
3. Run each code block and observe the output

Note: The code uses `getpass.getpass()` to safely request the token input when running in Colab.

---

## Token Security Notice

For security reasons, the GitHub token is not included in the notebook.

- A separate file named `TOKEN_SECURITY_NOTE.txt` is included in this repository, explaining why the token was not shared publicly.
- The notebook is fully functional and can be run with any GitHub Personal Access Token that includes the `public_repo` permission.

---

## Reflection

This practice helped me:

- Improve my understanding of how to use RESTful APIs in real scenarios
- Learn how to read and handle JSON responses
- Work with authentication using tokens
- Automate common data extraction tasks from public data sources
- Apply good security practices by not exposing sensitive credentials

---

## API Endpoints Used

- Search Repositories: `GET /search/repositories`
- Get Commits: `GET /repos/{owner}/{repo}/commits`
- Get File Contents: `GET /repos/{owner}/{repo}/contents/{path}`
- Check Rate Limit: `GET /rate_limit`

Official documentation: https://docs.github.com/en/rest

---

## Project Status

Notebook completed and tested  
Uploaded to GitHub in `/Content`  
Token security handled via Colab prompt and separate explanation file
