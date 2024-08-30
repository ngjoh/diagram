```mermaid
sequenceDiagram
    participant Customer
    participant WoltApp
    participant Restaurant
    participant Courier
    
    Customer->>WoltApp: Open App and Browse Restaurants
    Customer->>WoltApp: Select Pizza and Place Order
    WoltApp->>Restaurant: Send Order Details
    Restaurant-->>WoltApp: Confirm Order
    WoltApp-->>Customer: Order Confirmation Notification
    Restaurant->>Restaurant: Prepare Pizza
    Restaurant-->>WoltApp: Order Prepared
    WoltApp->>Courier: Assign Delivery Partner
    Courier-->>WoltApp: Accept Delivery Job
    Courier->>Restaurant: Arrive and Pick Up Order
    Courier-->>WoltApp: Confirm Pickup
    WoltApp-->>Customer: Real-Time Tracking Notification
    Courier->>Customer: Deliver Pizza
    Customer->>WoltApp: Confirm Order Receipt
    WoltApp-->>Courier: Process Payment and Tip
    WoltApp-->>Restaurant: Process Payment
    Customer->>WoltApp: Rate and Review Experience
    WoltApp->>Customer: Provide Support and Promotions

```
