# GitHub User Profile Fetcher

This is a simple, single-page web application that allows you to fetch the creation date of any GitHub user profile. It is built with HTML, Tailwind CSS for styling, and vanilla JavaScript for fetching data from the GitHub API.

## Features

*   Fetches GitHub user creation dates (`YYYY-MM-DD UTC`).
*   Responsive design using Tailwind CSS.
*   Supports optional GitHub Personal Access Token for higher rate limits.

## How to Use

1.  **Open `index.html` in your browser.**
    You can simply open the `index.html` file directly in any modern web browser.

2.  **Enter a GitHub Username:**
    Type a GitHub username (e.g., `octocat`, `github`) into the input field and click "Fetch Creation Date". The creation date of the profile will be displayed.

3.  **Using a GitHub Personal Access Token (Optional):**
    The GitHub API has rate limits for unauthenticated requests. If you encounter rate limit issues (e.g., `API rate limit exceeded`), you can provide a GitHub Personal Access Token (PAT) to increase your rate limits.

    **To use a PAT:**
    *   Generate a PAT from your GitHub settings (under "Developer settings" -> "Personal access tokens"). You typically only need `public_repo` scope for public user data, or no scope if you just want to authenticate.
    *   Append `?token=YOUR_TOKEN_HERE` to the URL in your browser's address bar.
        **Example:** `file:///path/to/your/index.html?token=ghp_YOUR_TOKEN_HERE`
        (Replace `ghp_YOUR_TOKEN_HERE` with your actual token).

    The application will automatically detect and use the token from the URL for API requests.

## Development

This project is a single-file application. No build steps are required.

*   `index.html`: Contains all the HTML structure, Tailwind CSS CDN link, and JavaScript logic.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
