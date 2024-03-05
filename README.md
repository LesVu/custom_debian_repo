# Debian Custom Repo

## Add The Repo

`curl -s --compressed "https://lesvu.github.io/custom_debian_repo/debian/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/lesvu_repo.gpg >/dev/null`

`sudo curl -s --compressed -o /etc/apt/sources.list.d/lesvu_repo.list "https://lesvu.github.io/custom_debian_repo/debian/lesvu_repo.list"
sudo apt update
`
