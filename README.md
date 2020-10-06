# PluginPQL
Paperless Query Language Plugin for SWV. Connect Webview JS with Android System and Storage.

## How it works?
PQL is as easier as it can get, simple push and pull of data. New information is pushed at the bottom of the DB and same for pull as new information is taken from the botttom.

## Creating new PQL Objects
```java
PQL pql = new PQL();
pql.write(...);
pql.list(...);
pql.read(...);
```

## Writing to DB
```java
pql.write(String id, String data, Context context);
```

## Listing Available Variables
```java
pql.list(int type);
/*
type: 1 = all variables
type: 2 = unique variables
*/
```

## Pull all DB
```java
pql.pull(Context context);
```

## Flush DB
To remove all the content from database file.
```java
pql.flush(Context context)
```
