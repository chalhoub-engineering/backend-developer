
# Backend Developer Test

Solve a problem as described below

We are working on connecting two systems. Lets call them `source` and `target` system

- Source system wants to call our API every time event occurs.
	- event structure `{ id: '<randomId>', name: 'test event', body: 'test body', timestamp: '<currentTimestamp>' }`
	- please mock the API calls from the source system

- Target system needs to recieve all the events
	- target system is an GraphQL API - please mock API calls to target system
	- event structure needs to be enchanced by adding `{ brand: 'testBrand' }` as target system requires it. Mind that this information is not flowing from source system
	- target system is rate limited. In most cases, events from source systems are flowing more frequent than target system is able to consume it. Please make sure designed solution will take that into consideration

### Considerations

- System needs to be working in the cloud
- Deployment must be through CI/CD pipeline
- System needs to be secure (authentication)
- System needs to be higly available
- We need to have full visibility about events flowing between `source` and `target` systems
- We need to be able to trace the flow of every single event
- Everything must be covered with tests
- Everything needs to be properly documented, with HLD and LLD included
- System needs to be easy to maintain and support
- All errors / issues need be visible and handled properly
- We want to see not only the solution but also how you think and your working process, so please keep all your commits accessible, dont squash them and use proper naming standard for them

### Required Technology

- Use Node (TypeScript) or GO as programming language
- Use Terraform to provision the infrastructure
- Use AWS or GCP

### Delivery

If your repository is private, please share it with daniel.rosiak@chalhoub.com and bilal.abdallah@faces.com
