## Database Design

The Smart Subscription Manager uses PostgreSQL as the primary relational database, hosted on Supabase.

🔗 Supabase Database Dashboard:
https://supabase.com/dashboard/project/wjljjcagednvkhevxdfp/database/schemas

### Core Tables
- users
- subscriptions
- categories
- notifications
- spending_history
- spending_predictions
- scanned_emails
- detected_services
- screen_time_entries

### Security
- Passwords are securely hashed before storage.
- JWT-based authentication is used.
- Row Level Security (RLS) is enabled to protect user data.
- Foreign key constraints ensure referential integrity.

### Database Features
- ENUM types for BillingCycle and SubscriptionStatus
- Indexed columns for performance optimization
- Cascade delete rules
- Prisma ORM used for schema migrations and version control
