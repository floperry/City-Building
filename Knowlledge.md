1.git usage

  a) add ssh key
  https://help.github.com/en/enterprise/2.15/user/articles/adding-a-new-ssh-key-to-your-github-account
  $ ls -al ~/.ssh
  # Lists the files in your .ssh directory, if they exist
  
  $ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
This creates a new ssh key, using the provided email as a label.

> Generating public/private rsa key pair.
When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

> Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa):[Press enter]
At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".

> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]

  type ssh-agent bash,if "Could not open a connection to your authentication agent"

  $ ssh-add ~/.ssh/id_rsa
  
  $ clip < ~/.ssh/id_rsa.pub
# Copies the contents of the id_rsa.pub file to your clipboard

  
  b)clone/commit/and push  
  https://rogerdudler.github.io/git-guide/
  git clone username@host:/path/to/repository
  
  
