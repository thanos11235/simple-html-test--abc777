# GitHub User Profile Fetcher

This is a simple web application that allows you to fetch and display public profile details for a GitHub user.

## Features

*   Fetch GitHub user's name, login, creation date, followers, following, public repositories, company, location, blog/website, bio, and avatar.
*   Uses the GitHub API.
*   Optionally accepts a GitHub personal access token via URL parameter to bypass rate limits.

## How to Use

1.  Open the `index.html` file in your web browser.
2.  Enter a GitHub username in the input field.
3.  Click the "Fetch Profile Details" button.
4.  The profile information will be displayed below the form.

### Using a GitHub Token (Optional)

To avoid GitHub API rate limiting for unauthenticated requests, you can provide a GitHub Personal Access Token (classic token with `public_repo` scope, or no scope if only fetching public data) as a URL query parameter. This is useful for development or testing.

Example:

`index.html?token=YOUR_GITHUB_PERSONAL_ACCESS_TOKEN`

**Note:** Do not share your personal access tokens publicly.

## Development

This project uses Tailwind CSS for styling, included via CDN.

The core logic is written in vanilla JavaScript to interact with the GitHub REST API (`https://api.github.com/users/{username}`).