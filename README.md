# About

This Nuxeo plugin provides an implementation of the BinaryManager that replies on MongoDB GridFS.

The goal is to store Nuxeo Blobs directly inside GridFS.

This is particularly interesting when using MongoDB as the main repository backend (using DBS) since this allows to have Structures + Meta-data and the Binaries inside the same MongoDB replicaSet.

# Building

    mvn clean install

# Testing

To run the tests, use '-Pitest' (or run from ftest/webdriver).

This requires:

- having a MongoDB server up and running; accessible through localhost. It can be overridden with `-Dnuxeo.mongodb.server=<IP>`

# Configuration

See [nuxeo-core-binarymanager-gridfs README](https://github.com/nuxeo/nuxeo-core-binarymanager-gridfs) for more informations.

# Specific Nuxeo Package Configuration

You are able to use some dedicated configuration properties for using another server for GridFS. If you do not want to use them; the mongodb server is configured with the default one.

See [default variables set with the Nuxeo Package](https://github.com/nuxeo/marketplace-binarymanager-gridfs/blob/master/marketplace/src/main/resources/install/templates/gridfsbinaries/nuxeo.defaults) for more informations.

# Resources

## Reporting issues

https://jira.nuxeo.com/browse/NXP/

# Licensing

[GNU Lesser General Public License (LGPL) v2.1](http://www.gnu.org/licenses/lgpl-2.1.html)

# About Nuxeo

Nuxeo dramatically improves how content-based applications are built, managed and deployed, making customers more agile, innovative and successful. Nuxeo provides a next generation, enterprise ready platform for building traditional and cutting-edge content oriented applications. Combining a powerful application development environment with
SaaS-based tools and a modular architecture, the Nuxeo Platform and Products provide clear business value to some of the most recognizable brands including Verizon, Electronic Arts, Netflix, Sharp, FICO, the U.S. Navy, and Boeing. Nuxeo is headquartered in New York and Paris.
More information is available at [www.nuxeo.com](http://www.nuxeo.com).
