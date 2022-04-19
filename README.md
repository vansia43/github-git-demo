# Git and GitHub Hands-On Demo Prerequisites

To get started with using Git and GitHub, you will need to install a few prerequisites on your system as well as create a GitHub account.

# Locally Install `git`

 1. From the Privileges application, click **Request Privileges**.

 1. Open a Terminal session, and check to see if you have `git` on your system:

    ```
    git --version
    ```
    If `git` is on your system, you will see a version number in the output, **and you do not need to complete the rest of the steps in this section.** If you get an error or a message asking whether you would like to install `git`, then follow the steps below to install it via Homebrew.

 1. Install [Homebrew](https://brew.sh/):

    ```
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    The script will walk you step by step through the installation process.

 1. Once Homebrew is installed, install `git`:

    ```
    brew install git
    ```

 1. Check if `git` was successfully installed:

    ```
    git --version
    ```
    This time, you should see a version number in the output. If for some reason it does not show the version number, close Terminal, restart, and run the command again.

 # Create a GitHub Account and Configure It Locally

 1. Go to [https://github.com/](https://github.com/) to sign up for an account.
 1. Verify your email address. Reference the [GitHub documentation](https://docs.github.com/en/get-started/signing-up-for-github/verifying-your-email-address) if you do not receive a verification email.
 1. Go back to Terminal, and configure `git` to use your credentials. Replace `Your_Name` with your actual name. Replace `Your_Email` with the email address you used to create your GitHub account (keep the quotes around these items):

    ```
    git config --global user.name "Your_Name"
    ```
    ```
    git config --global user.email "Your_Email"
    ```

# Create a Personal Access Token

 1. From the upper-right corner of your GitHub account, click your user icon and select **Settings**.
 1. Scroll down, and on the left, click **<> Developer settings**.
 1. From the left menu, select **Personal access tokens**.
 1. Click **Generate new token**.
 1. For *Note*, enter any name you want.
 1. For *Expiration*, choose whatever date you want. Once this token expires, you will have to create a new one.
 1. For *Select scopes*, check the box next to **repo**.
 1. Click **Generate token**.
 1. On the next page, you will see your new Personal Access Token. Copy that token to a text file — you will be unable to retrieve the token again after this screen. When you push files to GitHub from your machine, you will need to use this token when prompted for a password. Have the token handy at that time.
