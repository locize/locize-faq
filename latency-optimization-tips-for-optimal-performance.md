### What is latency?
Latency defines the time that is takes for a request to travel from the sender to the receiver and for the receiver to process that request.
This is greatly affected by how far away the user is from the server and the quality of the network.

### Latency optimization
You can never get rid of latency, but the great news is that there are latency optimization guidelines which you can apply to negate some of the delays that occur.

#### Our advice
1. Create a dedicated version for production ([How to add a new version?](/how-to-add-a-new-version.html))
2. Do not enable auto publish for that version and publish manually or via [API](https://docs.locize.com/api.html#publish-version)
3. Enable [Cache-Control max-age](https://docs.locize.com/caching.html)
