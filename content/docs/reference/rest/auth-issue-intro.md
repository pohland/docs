## <span class="post">POST</span> `/v1/auth/issue`

<aside class="note">
<strong>NOTE</strong>: This method is called on a DIFFERENT domain: <strong>https://auth.dfuse.io/v1/auth/issue</strong>
</aside>

First, obtain a long-term API key (go to https://app.dfuse.io).

> Sample request:

{{< highlight shell >}}
curl -XPOST \
     -H "Content-Type: application/json" \
     --data '{"api_key":"web_ebf6733085d83117b0ad7f9999bd169c"}' \
     "https://auth.dfuse.io/v1/auth/issue"
{{< /highlight >}}

### JSON payload input parameters

Name | Type | Options | Description
-----|------|---------|------------
`api_key` | string | **required** | Long-term API key

### Response

Returns a [AuthTokenResponse](#type-AuthTokenResponse).