<a href="http://projectdanube.org/" target="_blank"><img src="http://projectdanube.github.com/xdi2/images/projectdanube_logo.png" align="right"></a>
<img src="http://projectdanube.github.com/xdi2/images/logo64.png"><br>

This is a project to use the [Berkeley DB](https://www.oracle.com/database/berkeley-db/db.html) key/value store as backend storage for the [XDI2](http://github.com/projectdanube/xdi2) server.

### Information

* [Code Example](https://github.com/projectdanube/xdi2-bdb/wiki/Code%20Example)
* [Server Configuration Example](https://github.com/projectdanube/xdi2-bdb/wiki/Server%20Configuration%20Example)
* [Graph Factory Flags](https://github.com/projectdanube/xdi2-bdb/wiki/Graph%20Factory%20Flags)

### How to build

First, you need to build the main [XDI2](http://github.com/projectdanube/xdi2) project.

After that, just run

    mvn clean install

To build the XDI2 plugin.

### How to run as standalone web application

    mvn clean install jetty:run -P war

Then access the web interface at

	http://localhost:9996/

Or access the server's status page at

	http://localhost:9996/xdi

Or use an XDI client to send XDI messages to

    http://localhost:9996/xdi/graph

### Maven Dependency

	<dependency>
	    <groupId>xdi2</groupId>
	    <artifactId>xdi2-bdb</artifactId>
	    <version>${xdi2-bdb-version}</version>
	    <scope>compile</scope>
	</dependency>

### Community

Google Group: http://groups.google.com/group/xdi2

IRC: irc://irc.freenode.net:6667/xdi
