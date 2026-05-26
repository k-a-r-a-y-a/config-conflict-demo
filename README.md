# Config Conflict Demo - Environment Configuration Lab

## Purpose
Demonstrate merge conflict resolution for environment configuration files.

## Scenario
Two developers modified `config/app.env` simultaneously:
- **Student A**: Changed `APP_MODE=development`
- **Student B**: Changed `APP_MODE=production`

## Resolution Strategy
Kept both environments in **separate files** instead of choosing one.

### Final Files
config/
├── app.env.development (from Student A)
├── app.env.production (from Student B)
├── app.env.staging (bonus)
└── README.md
Key Learning
Never force push shared branches. Use git revert for production.
