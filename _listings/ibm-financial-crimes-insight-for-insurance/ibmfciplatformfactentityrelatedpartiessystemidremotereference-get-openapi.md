---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API This method is used to retrieve
    the set of explicitly related parties and implicitly related entities for the
    supplied externally sourced reference party
  description: |-
    A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:

    &lt;dataSource beginTranForResultSetScrollingAPIs="false" id="ISIIDB" isolationLevel="TRANSACTION_READ_COMMITTED" jndiName="jdbc/isii"&gt;

    &lt;jdbcDriver javax.sql.DataSource="com.ibm.db2.jcc.DB2XADataSource" libraryRef="DB2_LIB"/&gt;

    &lt;properties.db2.jcc databaseName="ISII" password="${isii_db_pass}" portNumber="${isii_db_port}" serverName="${isii_host}" user="${isii_db_user}"/&gt;

    &lt;connectionManager connectionTimeout="60s" maxIdleTime="3m" maxPoolSize="200" minPoolSize="0"/&gt;

    &lt;/dataSource&gt;

    Where password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/entity/relatedparties/{systemId}/{remoteReference}:
    get:
      summary: This method is used to retrieve the set of explicitly related parties
        and implicitly related entities for the supplied externally sourced reference
        party
      description: |-
        A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:

        &lt;dataSource beginTranForResultSetScrollingAPIs="false" id="ISIIDB" isolationLevel="TRANSACTION_READ_COMMITTED" jndiName="jdbc/isii"&gt;

        &lt;jdbcDriver javax.sql.DataSource="com.ibm.db2.jcc.DB2XADataSource" libraryRef="DB2_LIB"/&gt;

        &lt;properties.db2.jcc databaseName="ISII" password="${isii_db_pass}" portNumber="${isii_db_port}" serverName="${isii_host}" user="${isii_db_user}"/&gt;

        &lt;connectionManager connectionTimeout="60s" maxIdleTime="3m" maxPoolSize="200" minPoolSize="0"/&gt;

        &lt;/dataSource&gt;

        Where password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.
      operationId: getRelatedObjects
      x-api-path-slug: ibmfciplatformfactentityrelatedpartiessystemidremotereference-get
      parameters:
      - in: query
        name: minRelatedScore
        description: Minimum matching score for implicit relationships
      - in: path
        name: remoteReference
        description: Remote reference object key
      - in: path
        name: systemId
        description: Remote reference system ID
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Retrieve
      - Set
      - Of
      - Explicitly
      - Related
      - Parties
      - Implicitly
      - Related
      - Entitiesthe
      - Supplied
      - Externally
      - Sourced
      - Reference
      - Party
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---