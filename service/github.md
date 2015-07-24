## Usage

### Use access token instead of password

Creating an access token for command-line use.

1. [Create a personal access token](https://help.github.com/articles/creating-an-access-token-for-command-line-use/) on your application settings page.
2. Once you have a token, you can enter it instead of your password when performing Git operations over HTTPS

    ```bash
    git clone https://github.com/username/repo.git
    Username: your_username
    Password: your_token
    ```
3. Git automation with .netrc file.

    ```bash
    cat ~/.netrc
    machine github.com
    login your_username
    password your_token

    machine api.github.com
    login your_username
    password your_token
    ```
