---

copyright:
  years: 2015, 2017
lastupdated: "2017-04-25"

---

# {{site.data.keyword.SecureGateway}} Service Plans

With the release of v1.7.0, a new tiered plan pricing model was introduced that allows {{site.data.keyword.SecureGateway}} to scale to the needs of any company.  The table below provides the limitations associated with each of the publicly available plans:

![Tiered Plan Model](./images/planDetails.png?raw=true "Tiered Plan Model")

## Changing Plans
When you change plans, your new plan will be considered to be either an upgrade or a downgrade.  This is determined by the default number of gateways allowed by each plan (e.g., Professional (5) to Enterprise (25) is an upgrade).  When upgrading, there will be no service interruption; however, a downgrade will update all gateways to be [inactive](./securegateway_faq.html#states) which will require you to reactivate your gateways and destinations (up to your new plan limit) before service is restored.

<b>Note</b>: When transitioning from the Standard plan to any of the new plans, this will be considered a downgrade.


## Notification for limit exceeded
When you create the maximum allowed amount of gateway/destination, there will be a warning log shown in the dashboard of the gateway/destination.

When the amount of client is reached, and there is a new client attempt to connect to the gateway, there will be an error log shown in the client log, and the new client will be exited by the gateway.

When the data usage exceeds the data transfer allowance, there will be an error log shown in the client log, and the client will be exited by the gateway.
