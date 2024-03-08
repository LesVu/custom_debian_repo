# Debian Custom Repo

## Add The Repo

### Debian Repo
`curl -s --compressed "https://lesvu.github.io/custom_debian_repo/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/lesvu_repo.gpg >/dev/null && sudo curl -s --compressed -o /etc/apt/sources.list.d/lesvu_repo.list "https://lesvu.github.io/custom_debian_repo/lesvu_repo.list" && sudo apt update
`

`reprepro -V -b ./debian --confdir ./conf --section other -C <component> includedeb bookworm <deb>
`
