# HAPI-FHIR-JPASERVER

There is a complete sample work based on a GitHub repo here: [hapi-fhir-jpaserver-example](https://github.com/jamesagnew/hapi-fhir/tree/master/hapi-fhir-jpaserver-example)

HAPI FHIR server running on Tomcat using MySQL database

Edit MySQL configuration for your project in FhirServerConfig.java, e.g.:
```
public DataSource dataSource() {
	BasicDataSource retVal = new BasicDataSource();
	retVal.setDriver(new com.mysql.jdbc.Driver());
	retVal.setUrl("jdbc:mysql://localhost:3306/hapifhir");
	
	retVal.setUsername("root");
	retVal.setPassword("");
	return retVal;
	}
```

Edit the MySQL drivers in the pom.xml file if you have different version of MySQL, e.g.:
```
< dependency >
  < groupId > mysql </ groupId >
  < artifactId > mysql-connector-java </ artifactId >
  < version > 6.0.6 </ version >
</ dependency >
```
Browse your FHIR API server via http://localhost:8080/hapi-fhir-jpaserver/

