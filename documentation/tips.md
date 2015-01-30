## Random Tips and Snippets

### Redirect www to non www sites in Coldfusion

    <cfif cgi.SERVER_NAME contains "www">
    <cfset nstring = #CGI.QUERY_STRING#>
    <cfif cgi.SCRIPT_NAME contains "index.cfm">
    	<cfheader statuscode="301" statustext="Moved Permanently">
    		<cfif nstring is not "">
                  <cflocation url="http://gilpingivhan.com?#CGI.QUERY_STRING#" addtoken="no"/>
              <cfelse>
                  <cflocation url="http://gilpingivhan.com" addtoken="no"/>
              </cfif>
    	<cfabort>
    <cfelse>
    	<cfheader statuscode="301" statustext="Moved Permanently">
    		<cfif nstring is not "">
                  <cflocation url="http://gilpingivhan.com#cgi.SCRIPT_NAME#?#CGI.QUERY_STRING#" addtoken="no"/>
              <cfelse>
                  <cflocation url="http://gilpingivhan.com#cgi.SCRIPT_NAME#" addtoken="no"/>
              </cfif>
    	<cfabort>
    </cfif>
    </cfif>