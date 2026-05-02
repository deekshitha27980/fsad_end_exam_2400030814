# Delivery HQL Demo

This Maven project demonstrates Hibernate Query Language (HQL) operations on a `Delivery` entity.

## Package

- `com.klef.fsad.exam`

## Database

- Uses embedded H2 database; no external database installation is required
- The database file is created automatically in `fsad-end-sem/data`
- No changes are needed in `src/main/resources/hibernate.cfg.xml` unless you want a custom path

## Build

From the project root (`fsad-end-sem`):

```bash
cd "c:\Users\deeks\OneDrive\Desktop\pro connect clone-backend\fsad-end-sem"
mvn clean package
```

## Run

```bash
mvn exec:java -Dexec.mainClass=com.klef.fsad.exam.ClientDemo
```

Or run the assembled JAR:

```bash
java -jar target/delivery-hql-demo-1.0-SNAPSHOT-jar-with-dependencies.jar
```

## Behavior

- Inserts two `Delivery` records using persistent objects
- Deletes one record by ID using HQL with positional parameters
- Prints remaining deliveries
