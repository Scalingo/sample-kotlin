# Sample Kotlin

A Kotlin app, which can easily be deployed to Scalingo.

## Running Locally

Make sure you have Java and Maven installed.

```sh
$ git clone https://github.com/Scalingo/sample-kotlin.git
$ cd sample-kotlin
$ mvn install
$ java -jar build/libs/sample-kotlin-1.0.jar
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

If you're going to use a database, ensure you have a local `.env` file that reads something like this:

```
JDBC_DATABASE_URL=jdbc:postgresql://localhost:5432/java_database_name
```

## Deploying to Scalingo

```sh
$ scalingo create my-kotlin-app
$ git push scalingo master
```

Head to https://my-kotlin-app.scalingo.io

## Documentation

For more information about using Java and Kotlin on Scalingo, see this article:
[Java on Scalingo](https://doc.scalingo.com/languages/java/start).
