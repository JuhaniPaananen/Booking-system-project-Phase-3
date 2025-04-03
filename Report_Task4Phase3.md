
# ZAP by Checkmarx Scanning Report

Generated with [![The ZAP
logo](2025-04-03-ZAP-Report-/zap32x32.png){.zap-logo}ZAP](https://zaproxy.org)
on Thu 3 Apr 2025, at 15:16:59

ZAP Version: 2.16.1

ZAP by [Checkmarx](https://checkmarx.com/)


::: {role="main"}
::: {#contents .section .contents}
## Contents

1.  [About this report](#about-this-report)
    1.  [Report parameters](#report-parameters)
2.  [Summaries](#summaries)
    1.  [Alert counts by risk and confidence](#risk-confidence-counts)
    2.  [Alert counts by site and risk](#site-risk-counts)
    3.  [Alert counts by alert type](#alert-type-counts)
3.  [Alerts](#alerts)
    1.  [Risk=[Medium]{.risk-level}, Confidence=[Low]{.confidence-level}
        (1)](#alerts--risk-2-confidence-1)
    2.  [Risk=[Informational]{.risk-level},
        Confidence=[High]{.confidence-level}
        (1)](#alerts--risk-0-confidence-3)
    3.  [Risk=[Informational]{.risk-level},
        Confidence=[Medium]{.confidence-level}
        (2)](#alerts--risk-0-confidence-2)
4.  [Appendix](#appendix)
    1.  [Alert types](#alert-types)
:::

::: {#about-this-report .section .about-this-report}
## About this report

::: {#report-parameters .section}
### Report parameters

::: report-parameters--container
#### Contexts

No contexts were selected, so all contexts were included by default.

#### Sites

The following sites were included:

-   [http://localhost:8000]{.site}

(If no sites were selected, all sites were included by default.)

An included site must also be within one of the included contexts for
its data to be included in the report.

#### Risk levels

Included: [[High]{.risk-level}, [Medium]{.risk-level},
[Low]{.risk-level}, [Informational]{.risk-level}]{.included-risk-codes}

Excluded: None

#### Confidence levels

Included: [[User Confirmed]{.confidence-level},
[High]{.confidence-level}, [Medium]{.confidence-level},
[Low]{.confidence-level}]{.included-confidence-codes}

Excluded: [ [User Confirmed]{.confidence-level},
[High]{.confidence-level}, [Medium]{.confidence-level},
[Low]{.confidence-level}, [False
Positive]{.confidence-level}]{.included-confidence-codes}
:::
:::
:::

::: section
:::

::: {#summaries .section .summaries}
## Summaries

::: {#risk-confidence-counts .section}
### Alert counts by risk and confidence

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                         Confidence                                                                                                                                                             
  ------ --------------- ---------------------------------------- ----------------------------------------- ----------------------------------------- ----------------------------------------- -----------------------------------------
                         User Confirmed                           High                                      Medium                                    Low                                       Total

  Risk   High            0\                                       0\                                        0\                                        0\                                        0\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}

         Medium          0\                                       0\                                        0\                                        1\                                        1\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(25.0%)]{.additional-info-percentages}   [(25.0%)]{.additional-info-percentages}

         Low             0\                                       0\                                        0\                                        0\                                        0\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}

         Informational   0\                                       1\                                        2\                                        0\                                        3\
                         [(0.0%)]{.additional-info-percentages}   [(25.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(75.0%)]{.additional-info-percentages}

         Total           0\                                       1\                                        2\                                        1\                                        4\
                         [(0.0%)]{.additional-info-percentages}   [(25.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(25.0%)]{.additional-info-percentages}   [(100%)]{.additional-info-percentages}
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

  : This table shows the number of alerts for each level of risk and
  confidence included in the report.\
  (The percentages in brackets represent the count as a percentage of
  the total number of alerts included in the report, rounded to one
  decimal place.)
:::

::: {#site-risk-counts .section}
### Alert counts by site and risk

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                 Risk                                                                                                                  
  ------ ----------------------- -------------------------------------- ---------------------------------------- ------------------------------------- -----------------------------------------------
                                 High\                                  Medium\                                  Low\                                  Informational\
                                 [(=                                    [(\>=                                    [(\>=                                 [(\>=
                                 High)]{.additional-info-percentages}   Medium)]{.additional-info-percentages}   Low)]{.additional-info-percentages}   Informational)]{.additional-info-percentages}

  Site   http://localhost:8000   0\                                     1\                                       0\                                    3\
                                 [(0)]{.additional-info-percentages}    [(1)]{.additional-info-percentages}      [(1)]{.additional-info-percentages}   [(4)]{.additional-info-percentages}
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

  : This table shows, for each site for which one or more alerts were
  raised, the number of alerts raised at each risk level.\
  Alerts with a confidence level of \"False Positive\" have been
  excluded from these counts.\
  (The numbers in brackets are the number of alerts raised for the site
  at or above that risk level.)
:::

::: {#alert-type-counts .section}
### Alert counts by alert type

  -----------------------------------------------------------------------------------------------
  Alert type                   Risk                    Count
  ---------------------------- ----------------------- ------------------------------------------
  [Absence of Anti-CSRF        Medium                  1\
  Tokens](#alert-type-0)                               [(25.0%)]{.additional-info-percentages}

  [Authentication Request      Informational           2\
  Identified](#alert-type-1)                           [(50.0%)]{.additional-info-percentages}

  [Session Management Response Informational           20\
  Identified](#alert-type-2)                           [(500.0%)]{.additional-info-percentages}

  [User Agent                  Informational           24\
  Fuzzer](#alert-type-3)                               [(600.0%)]{.additional-info-percentages}

  Total                                                4
  -----------------------------------------------------------------------------------------------

  : This table shows the number of alerts of each alert type, together
  with the alert type\'s risk level.\
  (The percentages in brackets represent each count as a percentage,
  rounded to one decimal place, of the total number of alerts included
  in this report.)
:::
:::

::: {#alerts .section .alerts}
## Alerts

1.  ::: {#alerts--risk-2-confidence-1}
    ### Risk=[Medium]{.risk-level}, Confidence=[Low]{.confidence-level} (1)

    1.  #### [http://localhost:8000]{.site} (1)

        1.  ##### [Absence of Anti-CSRF Tokens](#alert-type-0) (1)

            1.  [GET
                http://localhost:8000/resources]{.request-method-n-url}
                +-----------------------------------+-----------------------------------+
                | Alert tags                        | -   [OWASP_                       |
                |                                   | 2021_A01](https://owasp.org/Top10 |
                |                                   | /A01_2021-Broken_Access_Control/) |
                |                                   | -   [WSTG-v42-SESS-05](htt        |
                |                                   | ps://owasp.org/www-project-web-se |
                |                                   | curity-testing-guide/v42/4-Web_Ap |
                |                                   | plication_Security_Testing/06-Ses |
                |                                   | sion_Management_Testing/05-Testin |
                |                                   | g_for_Cross_Site_Request_Forgery) |
                |                                   | -   [OWASP_2017_A05](https://owas |
                |                                   | p.org/www-project-top-ten/2017/A5 |
                |                                   | _2017-Broken_Access_Control.html) |
                |                                   | -   [CWE-352](https://cwe.mit     |
                |                                   | re.org/data/definitions/352.html) |
                +-----------------------------------+-----------------------------------+
                | Alert description                 | No Anti-CSRF tokens were found in |
                |                                   | a HTML submission form.           |
                |                                   |                                   |
                |                                   | A cross-site request forgery is   |
                |                                   | an attack that involves forcing a |
                |                                   | victim to send an HTTP request to |
                |                                   | a target destination without      |
                |                                   | their knowledge or intent in      |
                |                                   | order to perform an action as the |
                |                                   | victim. The underlying cause is   |
                |                                   | application functionality using   |
                |                                   | predictable URL/form actions in a |
                |                                   | repeatable way. The nature of the |
                |                                   | attack is that CSRF exploits the  |
                |                                   | trust that a web site has for a   |
                |                                   | user. By contrast, cross-site     |
                |                                   | scripting (XSS) exploits the      |
                |                                   | trust that a user has for a web   |
                |                                   | site. Like XSS, CSRF attacks are  |
                |                                   | not necessarily cross-site, but   |
                |                                   | they can be. Cross-site request   |
                |                                   | forgery is also known as CSRF,    |
                |                                   | XSRF, one-click attack, session   |
                |                                   | riding, confused deputy, and sea  |
                |                                   | surf.                             |
                |                                   |                                   |
                |                                   | CSRF attacks are effective in a   |
                |                                   | number of situations, including:  |
                |                                   |                                   |
                |                                   | \* The victim has an active       |
                |                                   | session on the target site.       |
                |                                   |                                   |
                |                                   | \* The victim is authenticated    |
                |                                   | via HTTP auth on the target site. |
                |                                   |                                   |
                |                                   | \* The victim is on the same      |
                |                                   | local network as the target site. |
                |                                   |                                   |
                |                                   | CSRF has primarily been used to   |
                |                                   | perform an action against a       |
                |                                   | target site using the victim\'s   |
                |                                   | privileges, but recent techniques |
                |                                   | have been discovered to disclose  |
                |                                   | information by gaining access to  |
                |                                   | the response. The risk of         |
                |                                   | information disclosure is         |
                |                                   | dramatically increased when the   |
                |                                   | target site is vulnerable to XSS, |
                |                                   | because XSS can be used as a      |
                |                                   | platform for CSRF, allowing the   |
                |                                   | attack to operate within the      |
                |                                   | bounds of the same-origin policy. |
                +-----------------------------------+-----------------------------------+
                | Other info                        | No known Anti-CSRF token          |
                |                                   | \[anticsrf, CSRFToken,            |
                |                                   | \_\_RequestVerificationToken,     |
                |                                   | csrfmiddlewaretoken,              |
                |                                   | authenticity_token,               |
                |                                   | OWASP_CSRFTOKEN, anoncsrf,        |
                |                                   | csrf_token, \_csrf, \_csrfSecret, |
                |                                   | \_\_csrf_magic, CSRF, \_token,    |
                |                                   | \_csrf_token, \_csrfToken\] was   |
                |                                   | found in the following HTML form: |
                |                                   | \[Form 1: \"resource_id\"         |
                |                                   | \"resource_name\" \].             |
                +-----------------------------------+-----------------------------------+
                | Request                           | Request line and header section   |
                |                                   | (573 bytes)                       |
                |                                   |     GET http://                   |
                |                                   | localhost:8000/resources HTTP/1.1 |
                |                                   |     host: localhost:8000          |
                |                                   |     User-Agent: Mozi              |
                |                                   | lla/5.0 (X11; Linux x86_64; rv:12 |
                |                                   | 8.0) Gecko/20100101 Firefox/128.0 |
                |                                   |     Accep                         |
                |                                   | t: text/html,application/xhtml+xm |
                |                                   | l,application/xml;q=0.9,*/*;q=0.8 |
                |                                   |                                   |
                |                                   |   Accept-Language: en-US,en;q=0.5 |
                |                                   |     Connection: keep-alive        |
                |                                   |                                   |
                |                                   |  Referer: https://localhost:8000/ |
                |                                   |     Cooki                         |
                |                                   | e: csrf_token=0fe636d7-da34-4eb0- |
                |                                   | 948b-a00cf41f8f4c; session_id=ba7 |
                |                                   | ec3be-b0ee-4ea6-91e7-b9dbc201028d |
                |                                   |     Upgrade-Insecure-Requests: 1  |
                |                                   |     Sec-Fetch-Dest: document      |
                |                                   |     Sec-Fetch-Mode: navigate      |
                |                                   |     Sec-Fetch-Site: same-origin   |
                |                                   |     Sec-Fetch-User: ?1            |
                |                                   |     Priority: u=0, i              |
                |                                   |                                   |
                |                                   | Request body (0 bytes)            |
                +-----------------------------------+-----------------------------------+
                | Response                          | Status line and header section    |
                |                                   | (325 bytes)                       |
                |                                   |     HTTP/1.1 200 OK               |
                |                                   |     content-type: text/html       |
                |                                   |     content-s                     |
                |                                   | ecurity-policy: default-src 'self |
                |                                   | '; script-src 'self'; style-src ' |
                |                                   | self'; img-src 'self'; frame-ance |
                |                                   | stors 'none'; form-action 'self'; |
                |                                   |     x-frame-options: DENY         |
                |                                   |                                   |
                |                                   |   x-content-type-options: nosniff |
                |                                   |     vary: Accept-Encoding         |
                |                                   |     content-length: 2235          |
                |                                   |     da                            |
                |                                   | te: Thu, 03 Apr 2025 11:04:05 GMT |
                |                                   |                                   |
                |                                   | Response body (2235 bytes)        |
                |                                   |     <!DOCTYPE html>               |
                |                                   |     <html lang="en">              |
                |                                   |     <head>                        |
                |                                   |         <meta charset="UTF-8">    |
                |                                   |         <met                      |
                |                                   | a name="viewport" content="width= |
                |                                   | device-width, initial-scale=1.0"> |
                |                                   |                                   |
                |                                   |   <title>Manage Resources</title> |
                |                                   |         <link href="/stati        |
                |                                   | c/tailwind.css" rel="stylesheet"> |
                |                                   |     </head>                       |
                |                                   |     <body c                       |
                |                                   | lass="bg-gray-100 text-gray-900"> |
                |                                   |         <d                        |
                |                                   | iv class="container mx-auto p-4"> |
                |                                   |             <di                   |
                |                                   | v class="bg-white shadow-md round |
                |                                   | ed-lg p-6 mt-6 max-w-xl mx-auto"> |
                |                                   |                 <h1               |
                |                                   |  class="text-2xl font-bold mb-4 t |
                |                                   | ext-center">Manage resources</h1> |
                |                                   |                 <form a           |
                |                                   | ction="/resources" method="POST"> |
                |                                   |                     <!-- Resourc  |
                |                                   | e ID (hidden for new entries) --> |
                |                                   |                                   |
                |                                   |          <input type="hidden" nam |
                |                                   | e="resource_id" id="resource_id"> |
                |                                   |                                   |
                |                                   |                                   |
                |                                   |            <!-- Resource Name --> |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                         <label    |
                |                                   | for="resource_name" class="block  |
                |                                   | text-sm font-medium text-gray-700 |
                |                                   |  font-bold">Resource Name</label> |
                |                                   |                         <input ty |
                |                                   | pe="text" name="resource_name" id |
                |                                   | ="resource_name" maxlength="100"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                                   |
                |                                   |     <!-- Resource Description --> |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |             <label for="resource_ |
                |                                   | description" class="block text-sm |
                |                                   |  font-medium text-gray-700 font-b |
                |                                   | old">Resource Description</label> |
                |                                   |                                   |
                |                                   |                <textarea name="re |
                |                                   | source_description" id="resource_ |
                |                                   | description" rows="4" required cl |
                |                                   | ass="mt-1 block w-full px-3 py-2  |
                |                                   | border border-gray-300 rounded-md |
                |                                   |  shadow-sm focus:outline-none foc |
                |                                   | us:ring-indigo-500 focus:border-i |
                |                                   | ndigo-500 sm:text-sm"></textarea> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                                   |
                |                                   |                  <!-- Buttons --> |
                |                                   |                     <div class=   |
                |                                   | "flex justify-between space-x-4"> |
                |                                   |                                   |
                |                                   |   <button type="submit" class="in |
                |                                   | line-block bg-blue-500 text-white |
                |                                   |  py-2 px-4 rounded hover:bg-blue- |
                |                                   | 600 w-1/2">Save Resource</button> |
                |                                   |                                   |
                |                                   |             <a href="/" class="in |
                |                                   | line-block bg-gray-500 text-white |
                |                                   |  text-center py-2 px-4 rounded ho |
                |                                   | ver:bg-gray-600 w-1/2">Cancel</a> |
                |                                   |                     </div>        |
                |                                   |                 </form>           |
                |                                   |             </div>                |
                |                                   |         </div>                    |
                |                                   |         <script src="/            |
                |                                   | static/resourceForm.js"></script> |
                |                                   |     </body>                       |
                |                                   |     </html>                       |
                +-----------------------------------+-----------------------------------+
                | Evidence                          |     <form a                       |
                |                                   | ction="/resources" method="POST"> |
                +-----------------------------------+-----------------------------------+
                | Solution                          | Phase: Architecture and Design    |
                |                                   |                                   |
                |                                   | Use a vetted library or framework |
                |                                   | that does not allow this weakness |
                |                                   | to occur or provides constructs   |
                |                                   | that make this weakness easier to |
                |                                   | avoid.                            |
                |                                   |                                   |
                |                                   | For example, use anti-CSRF        |
                |                                   | packages such as the OWASP        |
                |                                   | CSRFGuard.                        |
                |                                   |                                   |
                |                                   | Phase: Implementation             |
                |                                   |                                   |
                |                                   | Ensure that your application is   |
                |                                   | free of cross-site scripting      |
                |                                   | issues, because most CSRF         |
                |                                   | defenses can be bypassed using    |
                |                                   | attacker-controlled script.       |
                |                                   |                                   |
                |                                   | Phase: Architecture and Design    |
                |                                   |                                   |
                |                                   | Generate a unique nonce for each  |
                |                                   | form, place the nonce into the    |
                |                                   | form, and verify the nonce upon   |
                |                                   | receipt of the form. Be sure that |
                |                                   | the nonce is not predictable      |
                |                                   | (CWE-330).                        |
                |                                   |                                   |
                |                                   | Note that this can be bypassed    |
                |                                   | using XSS.                        |
                |                                   |                                   |
                |                                   | Identify especially dangerous     |
                |                                   | operations. When the user         |
                |                                   | performs a dangerous operation,   |
                |                                   | send a separate confirmation      |
                |                                   | request to ensure that the user   |
                |                                   | intended to perform that          |
                |                                   | operation.                        |
                |                                   |                                   |
                |                                   | Note that this can be bypassed    |
                |                                   | using XSS.                        |
                |                                   |                                   |
                |                                   | Use the ESAPI Session Management  |
                |                                   | control.                          |
                |                                   |                                   |
                |                                   | This control includes a component |
                |                                   | for CSRF.                         |
                |                                   |                                   |
                |                                   | Do not use the GET method for any |
                |                                   | request that triggers a state     |
                |                                   | change.                           |
                |                                   |                                   |
                |                                   | Phase: Implementation             |
                |                                   |                                   |
                |                                   | Check the HTTP Referer header to  |
                |                                   | see if the request originated     |
                |                                   | from an expected page. This could |
                |                                   | break legitimate functionality,   |
                |                                   | because users or proxies may have |
                |                                   | disabled sending the Referer for  |
                |                                   | privacy reasons.                  |
                +-----------------------------------+-----------------------------------+
    :::

2.  ::: {#alerts--risk-0-confidence-3}
    ### Risk=[Informational]{.risk-level}, Confidence=[High]{.confidence-level} (1)

    1.  #### [http://localhost:8000]{.site} (1)

        1.  ##### [Authentication Request Identified](#alert-type-1) (1)

            1.  [POST
                http://localhost:8000/login]{.request-method-n-url}
                +-----------------------------------+-----------------------------------+
                | Alert tags                        |                                   |
                +-----------------------------------+-----------------------------------+
                | Alert description                 | The given request has been        |
                |                                   | identified as an authentication   |
                |                                   | request. The \'Other Info\' field |
                |                                   | contains a set of key=value lines |
                |                                   | which identify any relevant       |
                |                                   | fields. If the request is in a    |
                |                                   | context which has an              |
                |                                   | Authentication Method set to      |
                |                                   | \"Auto-Detect\" then this rule    |
                |                                   | will change the authentication to |
                |                                   | match the request identified.     |
                +-----------------------------------+-----------------------------------+
                | Other info                        | userParam=username                |
                |                                   |                                   |
                |                                   | userValue=foo-bar@example.com     |
                |                                   |                                   |
                |                                   | passwordParam=password            |
                |                                   |                                   |
                |                                   | re                                |
                |                                   | ferer=http://localhost:8000/login |
                |                                   |                                   |
                |                                   | csrfToken=csrf_token              |
                +-----------------------------------+-----------------------------------+
                | Request                           | Request line and header section   |
                |                                   | (342 bytes)                       |
                |                                   |     POST htt                      |
                |                                   | p://localhost:8000/login HTTP/1.1 |
                |                                   |     host: localhost:8000          |
                |                                   |     user-agent: Mozilla/5.0       |
                |                                   | (Windows NT 10.0; Win64; x64) App |
                |                                   | leWebKit/537.36 (KHTML, like Geck |
                |                                   | o) Chrome/131.0.0.0 Safari/537.36 |
                |                                   |     pragma: no-cache              |
                |                                   |     cache-control: no-cache       |
                |                                   |     content-type:                 |
                |                                   | application/x-www-form-urlencoded |
                |                                   |     ref                           |
                |                                   | erer: http://localhost:8000/login |
                |                                   |     content-length: 91            |
                |                                   |                                   |
                |                                   | Request body (91 bytes)           |
                |                                   |     csrf_token=d26c176e-fd77-     |
                |                                   | 4b53-8fc0-387ee013b323&username=f |
                |                                   | oo-bar%40example.com&password=ZAP |
                +-----------------------------------+-----------------------------------+
                | Response                          | Status line and header section    |
                |                                   | (345 bytes)                       |
                |                                   |     HTTP/1.1 403 Forbidden        |
                |                                   |     conte                         |
                |                                   | nt-type: text/plain;charset=UTF-8 |
                |                                   |     content-s                     |
                |                                   | ecurity-policy: default-src 'self |
                |                                   | '; script-src 'self'; style-src ' |
                |                                   | self'; img-src 'self'; frame-ance |
                |                                   | stors 'none'; form-action 'self'; |
                |                                   |     x-frame-options: DENY         |
                |                                   |                                   |
                |                                   |   x-content-type-options: nosniff |
                |                                   |     vary: Accept-Encoding         |
                |                                   |     content-length: 18            |
                |                                   |     da                            |
                |                                   | te: Thu, 03 Apr 2025 10:08:43 GMT |
                |                                   |                                   |
                |                                   | Response body (18 bytes)          |
                |                                   |     Invalid CSRF Token            |
                +-----------------------------------+-----------------------------------+
                | Parameter                         |     username                      |
                +-----------------------------------+-----------------------------------+
                | Evidence                          |     password                      |
                +-----------------------------------+-----------------------------------+
                | Solution                          | This is an informational alert    |
                |                                   | rather than a vulnerability and   |
                |                                   | so there is nothing to fix.       |
                +-----------------------------------+-----------------------------------+
    :::

3.  ::: {#alerts--risk-0-confidence-2}
    ### Risk=[Informational]{.risk-level}, Confidence=[Medium]{.confidence-level} (2)

    1.  #### [http://localhost:8000]{.site} (2)

        1.  ##### [Session Management Response Identified](#alert-type-2) (1)

            1.  [GET http://localhost:8000/login]{.request-method-n-url}
                +-----------------------------------+-----------------------------------+
                | Alert tags                        |                                   |
                +-----------------------------------+-----------------------------------+
                | Alert description                 | The given response has been       |
                |                                   | identified as containing a        |
                |                                   | session management token. The     |
                |                                   | \'Other Info\' field contains a   |
                |                                   | set of header tokens that can be  |
                |                                   | used in the Header Based Session  |
                |                                   | Management Method. If the request |
                |                                   | is in a context which has a       |
                |                                   | Session Management Method set to  |
                |                                   | \"Auto-Detect\" then this rule    |
                |                                   | will change the session           |
                |                                   | management to use the tokens      |
                |                                   | identified.                       |
                +-----------------------------------+-----------------------------------+
                | Other info                        | cookie:csrf_token                 |
                +-----------------------------------+-----------------------------------+
                | Request                           | Request line and header section   |
                |                                   | (266 bytes)                       |
                |                                   |     GET htt                       |
                |                                   | p://localhost:8000/login HTTP/1.1 |
                |                                   |     host: localhost:8000          |
                |                                   |     user-agent: Mozilla/5.0       |
                |                                   | (Windows NT 10.0; Win64; x64) App |
                |                                   | leWebKit/537.36 (KHTML, like Geck |
                |                                   | o) Chrome/131.0.0.0 Safari/537.36 |
                |                                   |     pragma: no-cache              |
                |                                   |     cache-control: no-cache       |
                |                                   |                                   |
                |                                   |    referer: http://localhost:8000 |
                |                                   |                                   |
                |                                   | Request body (0 bytes)            |
                +-----------------------------------+-----------------------------------+
                | Response                          | Status line and header section    |
                |                                   | (429 bytes)                       |
                |                                   |     HTTP/1.1 200 OK               |
                |                                   |     content-type: text/html       |
                |                                   |     set                           |
                |                                   | -cookie: csrf_token=d26c176e-fd77 |
                |                                   | -4b53-8fc0-387ee013b323; HttpOnly |
                |                                   | ; SameSite=Strict; Path=/; Secure |
                |                                   |     content-s                     |
                |                                   | ecurity-policy: default-src 'self |
                |                                   | '; script-src 'self'; style-src ' |
                |                                   | self'; img-src 'self'; frame-ance |
                |                                   | stors 'none'; form-action 'self'; |
                |                                   |     x-frame-options: DENY         |
                |                                   |                                   |
                |                                   |   x-content-type-options: nosniff |
                |                                   |     vary: Accept-Encoding         |
                |                                   |     content-length: 1967          |
                |                                   |     da                            |
                |                                   | te: Thu, 03 Apr 2025 10:08:43 GMT |
                |                                   |                                   |
                |                                   | Response body (1967 bytes)        |
                |                                   |     <!DOCTYPE html>               |
                |                                   |     <html lang="en">              |
                |                                   |     <head>                        |
                |                                   |         <meta charset="UTF-8">    |
                |                                   |         <met                      |
                |                                   | a name="viewport" content="width= |
                |                                   | device-width, initial-scale=1.0"> |
                |                                   |         <title>User Login</title> |
                |                                   |         <link href="/stati        |
                |                                   | c/tailwind.css" rel="stylesheet"> |
                |                                   |     </head>                       |
                |                                   |     <body c                       |
                |                                   | lass="bg-gray-100 text-gray-900"> |
                |                                   |         <d                        |
                |                                   | iv class="container mx-auto p-4"> |
                |                                   |             <div                  |
                |                                   |  class="bg-white shadow-md rounde |
                |                                   | d-lg p-6  mt-6 max-w-lg mx-auto"> |
                |                                   |                                   |
                |                                   |         <h1 class="text-2xl font- |
                |                                   | bold mb-4 text-center">Login</h1> |
                |                                   |                 <fo               |
                |                                   | rm action="/login" method="POST"> |
                |                                   |                                   |
                |                                   |                <input type="hidde |
                |                                   | n" name="csrf_token" value="d26c1 |
                |                                   | 76e-fd77-4b53-8fc0-387ee013b323"> |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |       <label for="username" class |
                |                                   | ="block text-sm font-medium text- |
                |                                   | gray-700 font-bold">Email</label> |
                |                                   |                                   |
                |                                   |                   <input type="em |
                |                                   | ail" id="username" name="username |
                |                                   | " placeholder="Enter your email"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |    <label for="password" class="b |
                |                                   | lock text-sm font-medium text-gra |
                |                                   | y-700 font-bold">Password</label> |
                |                                   |                                   |
                |                                   |             <input type="password |
                |                                   | " id="password" name="password" p |
                |                                   | laceholder="Enter your password"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                     <div class=   |
                |                                   | "flex justify-between space-x-4"> |
                |                                   |                                   |
                |                                   |           <button type="submit" c |
                |                                   | lass="inline-block bg-blue-500 te |
                |                                   | xt-white py-2 px-4 rounded hover: |
                |                                   | bg-blue-600 w-1/2">Login</button> |
                |                                   |                                   |
                |                                   |             <a href="/" class="in |
                |                                   | line-block bg-gray-500 text-white |
                |                                   |  py-2 px-4 rounded hover:bg-gray- |
                |                                   | 600 w-1/2 text-center">Cancel</a> |
                |                                   |                     </div>        |
                |                                   |                 </form>           |
                |                                   |             </div>                |
                |                                   |         </div>                    |
                |                                   |     </body>                       |
                |                                   |     </html>                       |
                +-----------------------------------+-----------------------------------+
                | Parameter                         |     csrf_token                    |
                +-----------------------------------+-----------------------------------+
                | Evidence                          |     d26                           |
                |                                   | c176e-fd77-4b53-8fc0-387ee013b323 |
                +-----------------------------------+-----------------------------------+
                | Solution                          | This is an informational alert    |
                |                                   | rather than a vulnerability and   |
                |                                   | so there is nothing to fix.       |
                +-----------------------------------+-----------------------------------+

        2.  ##### [User Agent Fuzzer](#alert-type-3) (1)

            1.  [GET
                http://localhost:8000/register]{.request-method-n-url}
                +-----------------------------------+-----------------------------------+
                | Alert tags                        |                                   |
                +-----------------------------------+-----------------------------------+
                | Alert description                 | Check for differences in response |
                |                                   | based on fuzzed User Agent (eg.   |
                |                                   | mobile sites, access as a Search  |
                |                                   | Engine Crawler). Compares the     |
                |                                   | response statuscode and the       |
                |                                   | hashcode of the response body     |
                |                                   | with the original response.       |
                +-----------------------------------+-----------------------------------+
                | Request                           | Request line and header section   |
                |                                   | (208 bytes)                       |
                |                                   |     GET http:/                    |
                |                                   | /localhost:8000/register HTTP/1.1 |
                |                                   |     host: localhost:8000          |
                |                                   |     user-agent: Mozilla/4.0 (comp |
                |                                   | atible; MSIE 8.0; Windows NT 6.1) |
                |                                   |     pragma: no-cache              |
                |                                   |     cache-control: no-cache       |
                |                                   |                                   |
                |                                   |    referer: http://localhost:8000 |
                |                                   |                                   |
                |                                   | Request body (0 bytes)            |
                +-----------------------------------+-----------------------------------+
                | Response                          | Status line and header section    |
                |                                   | (429 bytes)                       |
                |                                   |     HTTP/1.1 200 OK               |
                |                                   |     content-type: text/html       |
                |                                   |     set                           |
                |                                   | -cookie: csrf_token=fb07e095-c8ad |
                |                                   | -4905-895f-73ac93c7c4ec; HttpOnly |
                |                                   | ; SameSite=Strict; Path=/; Secure |
                |                                   |     content-s                     |
                |                                   | ecurity-policy: default-src 'self |
                |                                   | '; script-src 'self'; style-src ' |
                |                                   | self'; img-src 'self'; frame-ance |
                |                                   | stors 'none'; form-action 'self'; |
                |                                   |     x-frame-options: DENY         |
                |                                   |                                   |
                |                                   |   x-content-type-options: nosniff |
                |                                   |     vary: Accept-Encoding         |
                |                                   |     content-length: 2978          |
                |                                   |     da                            |
                |                                   | te: Thu, 03 Apr 2025 10:12:05 GMT |
                |                                   |                                   |
                |                                   | Response body (2978 bytes)        |
                |                                   |     <!DOCTYPE html>               |
                |                                   |     <html lang="en">              |
                |                                   |                                   |
                |                                   |     <head>                        |
                |                                   |         <meta charset="UTF-8">    |
                |                                   |         <met                      |
                |                                   | a name="viewport" content="width= |
                |                                   | device-width, initial-scale=1.0"> |
                |                                   |                                   |
                |                                   |  <title>User Registration</title> |
                |                                   |         <link href="/st           |
                |                                   | atic/tailwind.css" rel="styleshee |
                |                                   | t"> <!-- Link to Tailwind CSS --> |
                |                                   |     </head>                       |
                |                                   |                                   |
                |                                   |     <body c                       |
                |                                   | lass="bg-gray-100 text-gray-900"> |
                |                                   |         <d                        |
                |                                   | iv class="container mx-auto p-4"> |
                |                                   |             <di                   |
                |                                   | v class="bg-white shadow-md round |
                |                                   | ed-lg p-6 mt-6 max-w-lg mx-auto"> |
                |                                   |                                   |
                |                                   |      <h1 class="text-2xl font-bol |
                |                                   | d mb-4 text-center">Register</h1> |
                |                                   |                 <form             |
                |                                   | action="/register" method="POST"> |
                |                                   |                                   |
                |                                   |                <input type="hidde |
                |                                   | n" name="csrf_token" value="fb07e |
                |                                   | 095-c8ad-4905-895f-73ac93c7c4ec"> |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |       <label for="username" class |
                |                                   | ="block text-sm font-medium text- |
                |                                   | gray-700 font-bold">Email</label> |
                |                                   |                                   |
                |                                   |  <input type="email" id="username |
                |                                   | " name="username" placeholder="En |
                |                                   | ter your email" required class="m |
                |                                   | t-1 block w-full px-3 py-2 border |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |    <label for="password" class="b |
                |                                   | lock text-sm font-medium text-gra |
                |                                   | y-700 font-bold">Password</label> |
                |                                   |                                   |
                |                                   |               <input type="passwo |
                |                                   | rd" id="password" name="password" |
                |                                   |  placeholder="Create a password"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |  <label for="birthdate" class="bl |
                |                                   | ock text-sm font-medium text-gray |
                |                                   | -700 font-bold">Birthdate</label> |
                |                                   |                                   |
                |                                   |                <input type="date" |
                |                                   |  id="birthdate" name="birthdate"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                     </div>        |
                |                                   |                                   |
                |                                   |                <div class="mb-4"> |
                |                                   |                                   |
                |                                   |            <label for="role" clas |
                |                                   | s="block text-sm font-medium text |
                |                                   | -gray-700 font-bold">Role</label> |
                |                                   |                                   |
                |                                   |    <select id="role" name="role"  |
                |                                   | required class="mt-1 block w-full |
                |                                   |  px-3 py-2 border border-gray-300 |
                |                                   |  rounded-md shadow-sm focus:outli |
                |                                   | ne-none focus:ring-indigo-500 foc |
                |                                   | us:border-indigo-500 sm:text-sm"> |
                |                                   |                                   |
                |                                   |                         <option v |
                |                                   | alue="reserver">Reserver</option> |
                |                                   |                                   |
                |                                   |               <option value="admi |
                |                                   | nistrator">Administrator</option> |
                |                                   |                         </select> |
                |                                   |                     </div>        |
                |                                   |                     <div class=   |
                |                                   | "flex justify-between space-x-4"> |
                |                                   |                                   |
                |                                   |        <button type="submit" clas |
                |                                   | s="inline-block bg-blue-500 text- |
                |                                   | white py-2 px-4 rounded hover:bg- |
                |                                   | blue-600 w-1/2">Register</button> |
                |                                   |                                   |
                |                                   |             <a href="/" class="in |
                |                                   | line-block bg-gray-500 text-white |
                |                                   |  py-2 px-4 rounded hover:bg-gray- |
                |                                   | 600 w-1/2 text-center">Cancel</a> |
                |                                   |                     </div>        |
                |                                   |                 </form>           |
                |                                   |             </div>                |
                |                                   |         </div>                    |
                |                                   |     </body>                       |
                |                                   |                                   |
                |                                   |     </html>                       |
                +-----------------------------------+-----------------------------------+
                | Parameter                         |     Header User-Agent             |
                +-----------------------------------+-----------------------------------+
                | Attack                            |     Mozilla/4.0 (comp             |
                |                                   | atible; MSIE 8.0; Windows NT 6.1) |
                +-----------------------------------+-----------------------------------+
    :::
:::

::: {#appendix .section .appendix}
## Appendix

::: {#alert-types .section .alert-types}
### Alert types

This section contains additional information on the types of alerts in
the report.

1.  ::: {#alert-type-0}
    #### Absence of Anti-CSRF Tokens

    +-----------------------------------+-----------------------------------+
    | Source                            | raised by a passive scanner       |
    |                                   | ([Absence of Anti-CSRF            |
    |                                   | Tokens](https://www               |
    |                                   | .zaproxy.org/docs/alerts/10202/)) |
    +-----------------------------------+-----------------------------------+
    | CWE ID                            | [352](https://cwe.mit             |
    |                                   | re.org/data/definitions/352.html) |
    +-----------------------------------+-----------------------------------+
    | WASC ID                           | 9                                 |
    +-----------------------------------+-----------------------------------+
    | Reference                         | 1.  <htt                          |
    |                                   | ps://cheatsheetseries.owasp.org/c |
    |                                   | heatsheets/Cross-Site_Request_For |
    |                                   | gery_Prevention_Cheat_Sheet.html> |
    |                                   | 2.  <https://cwe.mit              |
    |                                   | re.org/data/definitions/352.html> |
    +-----------------------------------+-----------------------------------+
    :::

2.  ::: {#alert-type-1}
    #### Authentication Request Identified

    +-----------------------------------+-----------------------------------+
    | Source                            | raised by a passive scanner       |
    |                                   | ([Authentication Request          |
    |                                   | Identified](https://www           |
    |                                   | .zaproxy.org/docs/alerts/10111/)) |
    +-----------------------------------+-----------------------------------+
    | Reference                         | 1.  <https://www.z                |
    |                                   | aproxy.org/docs/desktop/addons/au |
    |                                   | thentication-helper/auth-req-id/> |
    +-----------------------------------+-----------------------------------+
    :::

3.  ::: {#alert-type-2}
    #### Session Management Response Identified

    +-----------------------------------+-----------------------------------+
    | Source                            | raised by a passive scanner       |
    |                                   | ([Session Management Response     |
    |                                   | Identified](https://www           |
    |                                   | .zaproxy.org/docs/alerts/10112/)) |
    +-----------------------------------+-----------------------------------+
    | Reference                         | 1.  <https://www.zapr             |
    |                                   | oxy.org/docs/desktop/addons/authe |
    |                                   | ntication-helper/session-mgmt-id> |
    +-----------------------------------+-----------------------------------+
    :::

4.  ::: {#alert-type-3}
    #### User Agent Fuzzer

    +-----------------------------------+-----------------------------------+
    | Source                            | raised by an active scanner       |
    |                                   | ([User Agent                      |
    |                                   | Fuzzer](https://www               |
    |                                   | .zaproxy.org/docs/alerts/10104/)) |
    +-----------------------------------+-----------------------------------+
    | Reference                         | 1.  <https://owasp.org/wstg>      |
    +-----------------------------------+-----------------------------------+
    :::
:::
:::
:::
