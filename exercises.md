# Exercises

## Exercise 1: Setup

1. Make an account on [GitHub](https://github.com/).
2. Download git using the [official Git installation guide](https://git-scm.com/install/).
3. Open your terminal.
4. Set up your local machine with the name and email that you want to appear on every commit.

    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your_email@example.com"
    ```

5. Create a Secure Shell (SSH) key. This helps GitHub authenticate your commits.

    ```bash
    ssh-keygen -t ed25519 -c "your_email@example.com"
    ```

    When prompted to "Enter a file in which to save the key," you can press Enter to accept the default. (You could pick a different location, but I find that I can only remember the default location).
6. Print out the contents of the public key and copy it.

    ```bash
    cat /path/to/public/key
    ```

    The path to the public key, if you saved it in the default, is probably something like `/Users/username/.ssh/id_ed25519.pub` or `/home/username/.ssh/id_ed25519.pub`.
7. Add the SSH key to your GitHub account using the [official GitHub instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

Setup is complete! You are ready to start contributing.

## Exercise 2: Cloning a repo

