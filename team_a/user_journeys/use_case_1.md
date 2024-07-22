```mermaid
journey
    title UEFA Euro 2024 - tickets
    section User Self-Registeration
        Registers with email or 3rd party email provider: 3: User
        Receives confirmation by email: 3: User
    section Phase 1 - Lottery
        Goes to ticket portal: 5: User, Web Site
        Views tickets by date or city: 3: User
        Selects tickets for desired games: 3: User
        Choses categories for tickets: 3: User
        Submits the application: 3: User
        Receives confirmation by email: 3: User
    section Lottery Draw
        Draws from ticket requests for each fixture: 4: Back-office
        Sends notification to ticket winners: 6: Back-office
    section Payment
        Goes to the portal: 5: User, Web Site
        Selects payment method: 4: User    
        Pays the price for won tickets: 5: User
    section Ticket Confirmation
        Reviews the ticket payment and user's details: 3: UEFA, Back-office
        Confirms tickets: 5: UEFA
        Receives confirmation: 7: User
```