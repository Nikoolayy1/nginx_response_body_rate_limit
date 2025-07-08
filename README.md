For response body rate limit the subrequest option can be used where the javascript sends a subrequest " let res = await r.subrequest('/backend'); " but I don't recomment it as seems to not scale well. Also the response then seems to be with the wrong header but then the in the internal location the " function header(r) { r.headersOut['Content-Type'] = "text/html";} " can be used to fix this.


![image](https://github.com/user-attachments/assets/066cf6d3-9dca-4535-9497-dd183ef0c43e)

