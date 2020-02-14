# CAP LIVECHAT SF 💻 [![Generic badge](https://img.shields.io/badge/CAP-Active-<COLOR>.svg)](https://shields.io/) 

Create a chat using SalesForce and Angular  

## **Previous requirements**

Before installing this package into your Angular application, you must be configured the live agent into your salesforce application. Follow this [link](https://help.salesforce.com/articleView?id=snapins_chat_setup.htm&type=5) for more instructions.

### Installation

``` npm install cap ```

### **Implementation into a module**

``` 
import { CapLiveChatModule } from 'cap-livechat';

@NgModule({
  declarations: [
    ...
  ],
  imports: [
    ...
    CapLiveChatModule.forRoot({
      embeddedServiceName: 'Your embedded service name',
      idServiceName: 'Your ID service name',
      urlSandbox: 'Your URL Sandbox',
      urlDomain: 'Your URL Domain',
      baseLiveAgentContentURL: 'Your base live agent content URL',
      deploymentId: 'Your deployment ID',
      buttonId: 'Your button ID',
      baseLiveAgentURL: 'Your base live agent URL',
      scriptUrl: 'Your script URL',
      eswLiveAgentDevName: 'Your esw live Agent Dev Name'
    })
  ]
})

```

### **HTML tags**

`<cap-live-chat-sf></cap-live-chat-sf>` 

![Alt text](https://github.com/software-allies/cap-livechat/blob/development/assets/images/cap-livechat.png?raw=true "caplivechat")

### **Local test**

In case that you don't have a domain and you want to test the CapLiveChat package we recomend you [ngrok](https://ngrok.com/). ``Ngrok`` provide a multiplatform tunnelling, reverse proxy software that establishes secure tunnels from a public endpoint such as internet to a locally running network service while capturing all traffic for detailed inspection and replay. For detailed inspection and replay. Follow this [link](https://www.npmjs.com/package/ngrok) for more instructions.
