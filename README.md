# signed-commits
Repository to practice signed commits

```
brew install gpg
gpg --version

gpg --list-secret-keys --keyid-format=long

gpg --full-generate-key
gpg --list-secret-keys --keyid-format=long

gpg --armor --export <key-id>
```

Signing commits:
```
git commit -S -m "Second commit"
git log --show-signature
```

Signing tags:
```
git tag --list
git tag v1 -m "demo v1"
git show v1

git tag -s v2 -m "demo tag"
git show v2

git push --tags
```

Based on 
https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key
https://docs.github.com/en/authentication/managing-commit-signature-verification/displaying-verification-statuses-for-all-of-your-commits


Another interesting material is https://www.youtube.com/watch?v=4166ExAnxmo
