# MongoDB with Docker Example

This example shows how to **set up Prisma using Docker and MongoDB** locally on your machine. It then uses the Prisma client in a simple Node script to read and write data in the database.

> When using MongoDB with Prisma, you use a [new datamodel format](https://www.prisma.io/docs/-b6a7/). Learn more in the [docs](https://www.prisma.io/docs/-b6o5/).

__INLINE(../_setup-1.md)__
cd prisma-examples/node/docker-mongodb
npm install
```

### 2. Launch Prisma with Docker

This example is based on Docker. If you don't have Docker installed, you can get it from [here](https://store.docker.com/search?type=edition&offering=community). Use the Docker Compose CLI to launch the Docker containers specified in [docker-compose.yml](./docker-compose.yml):

```
docker-compose up -d
```

### 3. Install the Prisma CLI

To run the example, you need the Prisma CLI. Please install it via NPM or [using another method](https://www.prisma.io/docs/prisma-cli-and-configuration/using-the-prisma-cli-alx4/#installation):

```
npm install -g prisma
```

### 4. Set up database & deploy Prisma datamodel

To deploy the datamodel for this example, run the following command:

```
prisma deploy
```

### 5. Run the script

Execute the script with this command: 

```
npm run start
```

__INLINE(../_next-steps.md)__