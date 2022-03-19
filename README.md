# mern_crud
set up MongoDB in mac os
  1. Install brew- /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  2. Check the version- brew -v
  3. Find MongoDB tap on Brew- brew tap mongodb/brew
  4. Install MongoDB community server- brew install mongodb-community
  5. Create DB folder on mac- sudo mkdir -p /System/Volumes/Data/data/db (beacuse apple creates new volume for security)
  6. Set permissions to use the db- sudo chown -R \`id -un\` /System/Volumes/Data/data/db
  7. Launch MongoDB- sudo mongod --dbpath /System/Volumes/Data/data/db
  8. set alias for this command- alias mongod='sudo mongod --dbpath /System/Volumes/Data/data/db'
  9. to launch mongodb- mongod
