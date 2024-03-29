# Next + Hono Quick Start

---

Uses:

-   [Tailwind CSS](https://tailwindcss.com/) for styling
-   [Shadcn](https://ui.shadcn.com/), [Radix](https://www.radix-ui.com/), [input-otp](https://input-otp.rodz.dev/), [Sonner](https://sonner.emilkowal.ski/), etc. for the UI components
-   [Hono](https://hono.dev/) as the API framework
-   [Scalar](https://docs.scalar.com/swagger-editor) as the Swagger Editor
-   [Drizzle](https://orm.drizzle.team/) as the ORM
-   [Postgres](https://www.postgresql.org/) as the database
-   [Lucia](https://lucia-auth.com/) and [Oslo](https://oslo.js.org/) for auth
-   [React Email](https://react.email/) for the email templates

## Getting Started (Dev)

-   Create a database on your local postgres instance called `example`.
-   Then run:

```bash
pnpm db:push
pnpm dev
```

## Note

Hono's Zod to OpenAPI package generates OpenAPI schema at `/api/swagger.json` and playground at `/api/scalar`.


## Env Vars

| Name               | Description                                                                   |
| ------------------ | ----------------------------------------------------------------------------- |
| NEXT_PUBLIC_DOMAIN | The domain of the website, defaults to localhost:3000                         |
| DATABASE_URL       | Postgres connection string, defaults to postgres://postgres@localhost/example |
| EMAIL_FROM         | Email from address, defaults to "Example <hey@example.com>"                   |
| EMAIL_PROVIDER     | Email provider, console, smtp, resend, default is console                     |
| RESEND_API_KEY     | If email provider is resend, get your key from resend.com                     |
| SMTP_HOST          | If email provider is smtp                                                     |
| SMTP_PORT          | If email provider is smtp, defaults to 587                                    |
| SMTP_USERNAME      | If email provider is smtp                                                     |
| SMTP_PASSWORD      | If email provider is smtp                                                     |
| SMTP_SECURE        | If email provider is smtp, true or 1, defaults to true                        |
