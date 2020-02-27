# What is HBase?

- Column store database
- Created as part of Apache project

# Why use HBase?

- Optimized for Querying
- Storage and writing is very fast
- Data is versioned
- Your data can be sparse (not all rows will have the same column entries)
- Data is sorted by row key

# How is the Data Stored?

HBase is made for distributed file systems, in particular, Hadoop.

# HBase is a little primitive

Compared to Relational Databases, we often use *denormalized* data because it is faster to access

# Versioning

A *cell* not only contains a value, but also a *timestamp*. 

Tables in HBase are versioned.

# The architecture of HBase

# Column Families

# Setup

Add these lines to your `~/.bashrc`:

```
#this is where the hbase shell lives
export HBASE_HOME="/home/courses/BMI535/students/hbase/hbase-1.2.6/"  
export PATH="$PATH:$HBASE_HOME/bin"
#need to add JAVA_HOME to make sure it runs
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64/
export PATH="$PATH:$JAVA_HOME/bin"
```

Remember to

```
source ~/.bashrc
```

# Opening up the HBase Shell

Once you have the above setup, you can open the HBase Shell by running:

```
hbase shell
```

# Creating your own namespace

A namespace is a place of your very own in the HBase database. It helps you avoid what are called *namespace* collisions.

One example of a *namespace collision* is if multiple users tried to create a table called `Gene` in the main workspace. There would be lots of errors.

So you can create your own namespace in HBase by running

```
create_namespace laderast
```

# Creating an HBase Table



# HBase versus Hive
