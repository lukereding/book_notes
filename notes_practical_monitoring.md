# Practical monitoring

Julian


## Anti-patterns

1. Tool obsession. Monitoring is super varied and complex. It doesn't help to get fixated on using a specific tool to use. Don't obsess over a tool because "Team X uses tool Y and team X is doing amazing; therefore if we use tool Y we will also be able to do amazing things" (aka _cargo cult monitoring_). In some cases, you might have to build new things. That's okay. And finally, _the single pane of glass_, i.e., a single place were you go to see all monitoring, is a myth. "...attempting to shoehorn everything into one tool or dashboard system is just going to hamper your ability to work effectively."
2. Monitoring as a job. How can you build monitoring for something you don't understand? Inherently, the people building the monitoring have to have some skin in the game and understand enough about the system they're monitoring, otherwise they will build crap.
3. Checkbox monitoring. Monitoring for the sake of monitoring, i.e., so you can check off a 'monitoring' box.
4. Using monitoring as a crutch. There is a tendency to put monitoring around specific things that break, instead of fixing the problem to begin with. Invest time in fixing the root cause instead of putting monitoring around a janky process.
5. Manual configuration


## Design patterns

1. Composable monitoring. "Use multiple specialized tools and couple them loosely together, forming a monitoring 'platform'." It's okay to have several monitoring tools, each of which does one thing well, that you 'compose' together.
2. Monitoring from the user's perspective. This is more for customer-facing applications.
3. Buy, don't build. Monitoring tools are usually not a source of competitive advantage.
4. Continual improvement. 

## Alerts

- Alerts are one way we accomplish the core goals of monitoring, i.e., observing and checking the inputs and outputs of a system and its components over time
- Two types of alerts:
  - Wake someone up
  - FYI
- He mostly focuses on the 'wake someone up' variety, but there are some general good patterns here
- Suggestions:
  - Stop using email for alerts. Leads to alert fatigue, overwhelms people with noise
  - Write runbooks. When things go wrong, write down who is responsible for the thing that's failing, what the component / service is, dependencies, what the logs and metrics means, what alerts are set up
  - Static thresholds aren't the only way.
  - Delete and tune alerts
  - Attempt self-healing at first


## Other notes

Components of a monitoring service (useful framework):
- Data collection
- Data storage
- Visualization
- Analytics and reporting
- Alerting

"The best dashboard focus on displaying the statis of a single service...or one product...These dashboards are most effective if they are created and maintained by the people that understand the service best."

Start with monitoring the core business KPIs that the business ultimately cares about. These are ultimately what higher-ups care about, and issues here can lead you to look at specific components of the broader system that may not be working.

"Monitoring isn't something that can be bolted on after the fact"