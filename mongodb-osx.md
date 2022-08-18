# Install MongoDB Community Edition on macOS
Please reference the official MongoDB Manual for installation [here](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/).
> Note: This README covers installing MongoDB Community Edition on macOS. If you use an alternate operating system, please follow the official guide here: https://docs.mongodb.com/manual/installation/

## In your terminal execute the following commands in order:

> Note: You can execute these commands in any directory in your terminal since we are installing MongoDB Server globally on your machine.

This will setup the brew library for MongoDB:

```sh
brew tap mongodb/brew
```

The below command will install the MongoDB Server on your machine:

```sh
brew install mongodb-community
```

For M1 users run the following instead:

```sh
arch -x86_64 /bin/bash -c "brew install mongodb-community"
```

The following command wil run the MongoDB Server in the background on your machine:
```sh
brew services start mongodb-community
```

To make sure that the MongoDB Community Server was installed correctly, run the following in your terminal:

```sh
brew services list
```

And you should see MongoDB Server running in that list.

### Troubleshooting

- https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/
