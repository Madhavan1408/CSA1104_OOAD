# CRC Cards — Home Appliance Control System (HACS)

## Homeowner
- **Responsibilities:** Request appliance actions; view device status
- **Collaborators:** MobileApp, Appliance

## MobileApp
- **Responsibilities:** Authenticate user; send commands; show status
- **Collaborators:** Homeowner, HomeGateway

## HomeGateway
- **Responsibilities:** Validate and route commands; report device state
- **Collaborators:** MobileApp, Appliance

## Appliance
- **Responsibilities:** Execute supported actions; expose current state
- **Collaborators:** HomeGateway

## AutomationRule
- **Responsibilities:** Store schedule/condition; trigger commands
- **Collaborators:** HomeGateway, Command

## Command
- **Responsibilities:** Represent action, target and execution result
- **Collaborators:** MobileApp, HomeGateway, Appliance

