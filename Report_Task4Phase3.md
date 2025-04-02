
# ZAP by Checkmarx Scanning Report

Generated with [![The ZAP
logo](2025-04-02-ZAP-Report-/zap32x32.png){.zap-logo}ZAP](https://zaproxy.org)
on Wed 2 Apr 2025, at 22:47:27

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
    1.  [Risk=[Informational]{.risk-level},
        Confidence=[High]{.confidence-level}
        (1)](#alerts--risk-0-confidence-3)
    2.  [Risk=[Informational]{.risk-level},
        Confidence=[Medium]{.confidence-level}
        (1)](#alerts--risk-0-confidence-2)
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
  ------ --------------- ---------------------------------------- ----------------------------------------- ----------------------------------------- ---------------------------------------- ------------------------------------------
                         User Confirmed                           High                                      Medium                                    Low                                      Total

  Risk   High            0\                                       0\                                        0\                                        0\                                       0\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}

         Medium          0\                                       0\                                        0\                                        0\                                       0\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}

         Low             0\                                       0\                                        0\                                        0\                                       0\
                         [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}    [(0.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}

         Informational   0\                                       1\                                        1\                                        0\                                       2\
                         [(0.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}   [(100.0%)]{.additional-info-percentages}

         Total           0\                                       1\                                        1\                                        0\                                       2\
                         [(0.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(50.0%)]{.additional-info-percentages}   [(0.0%)]{.additional-info-percentages}   [(100%)]{.additional-info-percentages}
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

  Site   http://localhost:8000   0\                                     0\                                       0\                                    2\
                                 [(0)]{.additional-info-percentages}    [(0)]{.additional-info-percentages}      [(0)]{.additional-info-percentages}   [(2)]{.additional-info-percentages}
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
  [Authentication Request      Informational           2\
  Identified](#alert-type-0)                           [(100.0%)]{.additional-info-percentages}

  [Session Management Response Informational           9\
  Identified](#alert-type-1)                           [(450.0%)]{.additional-info-percentages}

  Total                                                2
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

1.  ::: {#alerts--risk-0-confidence-3}
    ### Risk=[Informational]{.risk-level}, Confidence=[High]{.confidence-level} (1)

    1.  #### [http://localhost:8000]{.site} (1)

        1.  ##### [Authentication Request Identified](#alert-type-0) (1)

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
                |                                   | userValue=quest2@gmail.com        |
                |                                   |                                   |
                |                                   | passwordParam=password            |
                |                                   |                                   |
                |                                   | re                                |
                |                                   | ferer=http://localhost:8000/login |
                |                                   |                                   |
                |                                   | csrfToken=csrf_token              |
                +-----------------------------------+-----------------------------------+
                | Request                           | Request line and header section   |
                |                                   | (467 bytes)                       |
                |                                   |     POST htt                      |
                |                                   | p://localhost:8000/login HTTP/1.1 |
                |                                   |     host: localhost:8000          |
                |                                   |     User-Agent: Mozi              |
                |                                   | lla/5.0 (X11; Linux x86_64; rv:12 |
                |                                   | 8.0) Gecko/20100101 Firefox/128.0 |
                |                                   |     Accep                         |
                |                                   | t: text/html,application/xhtml+xm |
                |                                   | l,application/xml;q=0.9,*/*;q=0.8 |
                |                                   |                                   |
                |                                   |   Accept-Language: en-US,en;q=0.5 |
                |                                   |     Content-Type:                 |
                |                                   | application/x-www-form-urlencoded |
                |                                   |     Content-Length: 93            |
                |                                   |     Origin: http://localhost:8000 |
                |                                   |     Connection: keep-alive        |
                |                                   |     Ref                           |
                |                                   | erer: http://localhost:8000/login |
                |                                   |     Upgrade-Insecure-Requests: 1  |
                |                                   |     Priority: u=0, i              |
                |                                   |                                   |
                |                                   | Request body (93 bytes)           |
                |                                   |     csrf_token=dfb8bcdf-a252-40   |
                |                                   | 7a-b9a9-4e3801f73dcf&username=que |
                |                                   | st2%40gmail.com&password=quest123 |
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
                |                                   | te: Wed, 02 Apr 2025 19:00:16 GMT |
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

2.  ::: {#alerts--risk-0-confidence-2}
    ### Risk=[Informational]{.risk-level}, Confidence=[Medium]{.confidence-level} (1)

    1.  #### [http://localhost:8000]{.site} (1)

        1.  ##### [Session Management Response Identified](#alert-type-1) (1)

            1.  [GET
                http://localhost:8000/register]{.request-method-n-url}
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
                |                                   | (364 bytes)                       |
                |                                   |     GET http:/                    |
                |                                   | /localhost:8000/register HTTP/1.1 |
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
                |                                   |   Referer: http://localhost:8000/ |
                |                                   |     Upgrade-Insecure-Requests: 1  |
                |                                   |     Priority: u=0, i              |
                |                                   |                                   |
                |                                   | Request body (0 bytes)            |
                +-----------------------------------+-----------------------------------+
                | Response                          | Status line and header section    |
                |                                   | (429 bytes)                       |
                |                                   |     HTTP/1.1 200 OK               |
                |                                   |     content-type: text/html       |
                |                                   |     set                           |
                |                                   | -cookie: csrf_token=e8f96fa7-38e3 |
                |                                   | -4ce9-9e8b-af5cbded9ca1; HttpOnly |
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
                |                                   | te: Wed, 02 Apr 2025 18:59:26 GMT |
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
                |                                   | n" name="csrf_token" value="e8f96 |
                |                                   | fa7-38e3-4ce9-9e8b-af5cbded9ca1"> |
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
                | Parameter                         |     csrf_token                    |
                +-----------------------------------+-----------------------------------+
                | Evidence                          |     e8f                           |
                |                                   | 96fa7-38e3-4ce9-9e8b-af5cbded9ca1 |
                +-----------------------------------+-----------------------------------+
                | Solution                          | This is an informational alert    |
                |                                   | rather than a vulnerability and   |
                |                                   | so there is nothing to fix.       |
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

2.  ::: {#alert-type-1}
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
:::
:::
:::
