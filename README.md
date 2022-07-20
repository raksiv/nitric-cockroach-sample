## Description

Any cloud example of connecting to Cockroach DB using postgres - 

## Usage

### Step 1: Create a cockroach labs account  

Sign up for a free Cockroach Labs account and create a Serverless Cluster.
Create an SQL User and then retrieve your connection URL.

If stuck, follow step 1 from this [guide](https://www.cockroachlabs.com/docs/v22.1/deploy-lambda-function.html).

### Step 2: Install Nitric

<details>
 <summary>Prerequisites</summary>

- [Git](https://git-scm.com/)
- [Docker](https://docs.docker.com/get-docker/)
- [Pulumi](https://www.pulumi.com/docs/reference/cli/)

</details>

<details>
 <summary>MacOs</summary>

Install with [homebrew](https://brew.sh/)

```bash
brew install nitrictech/tap/nitric
```

</details>

<details>
 <summary>Windows</summary>

Install with [scoop](https://scoop.sh/)

```
scoop bucket add nitric https://github.com/nitrictech/scoop-bucket.git
scoop install nitric
```

</details>

<details>
 <summary>Linux</summary>
 
Download as a scripted install via curl.

```bash
curl https://nitric.io/install | bash

```

 </details>

<br/>

> Note: Complete installation guide can be found [here](https://nitric.io/docs/installation)

<br/>

### Step 3: Run the API locally with Nitric

```bash
yarn install
nitric run
```

### Step 4: Consume the API

```bash
curl http://localhost:9001/apis/main/init
```

```bash
{"message":"Database initialized"}% 
```

Login to Cockroach or query your database to confirm the changes.

## What's next?

Explore the [Nitric framework](https://nitric.io/docs) to learn how to deploy to the cloud and much more.
