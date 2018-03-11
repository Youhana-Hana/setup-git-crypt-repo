# setup-git-crypt-repo

To create an encrypted  git repository, you can use setup-encrypted-repo bash file

# Running it
"./setup-encrypted-repo -u new-git-repo-url -n gpg-key-name -k gpg-private-key

## Script takes the following parameters:
1. u	Full git repositpry URL including the new repository name
2. n	gpg key name
3. k	gpg private kry content without BEGIn & END Blocks


# Example
`./setup-encrypted-repo -u git@172.27.204.125:ert001/automation/configuration.git -n ConcourseCI -k LoejU***********************==k876`

# Script will do the following:
1. Create remote git repository
2. Add initial .gitattributes to encrypt YML and JSON files
3. Push changes to remote repo
4. Configure git-crypt
