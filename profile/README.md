
# Hey There! We're Sharing Excess, and we're building software to solve scarcity with surplus.

Sharing Excess is a 501(c)(3) nonprofit organization based in Philadelphia, PA. We work across the country to fight food insecurity by redistributing surplus food from farms, wholesalers, and retailers to local community hunger organizations. Since 2018, we've managed the distribution of over 150 million lbs. of food to our network of over 1,500 community partners in Philadelphia, New York, Washington DC, Chicago, Detroit, Los Angeles, and across the country.

Learn more about Sharing Excess at [sharingexcess.com](https://sharingexcess.com).

## Our Team

Tech @ Sharing Excess is a team of volunteers, students, part and full-time contributors. We work to build tools that enable SE to create impact across the country in a way that's efficient, transparent, and deeply measurable. We work hard to build a community based on collaborative learning, constant exploration, and easy-to-read code that makes it easy for new folks to jump in and help.

### Current Contributors

Ryan McHenry: [@ryanmarshallmc](https://github.com/ryanmarshallmc)
Tate Gallagher: [@tategallagher](https://github.com/tategallagher)
Satwik Shresth: [@satwikShresth](https://github.com/satwikShresth)

### Tech Team Mission

Tech@SE works to make food rescue as simple and transparent as possible. We design and develop tools to provide a shared language and framework for rescuing food, connecting our food donors, recipients, staff, and philanthropic funders with all of the information they need to get people fed. We provide our partners and funders with best-in-class data and insights, enabling us to build a continuously expanding network that is easy to join, and even easier to support.

### Tech Team Values

#### Simplicity
Food rescue is inherently complex, and incredibly dynamic. We strive to build products that are clear, logical, and easy to understand for first-time users and industry veterans alike.

#### Clarity
Sharing Excess's mission requires the support of partners and funders, and we continuously work to earn their trust by providing an unmatched level of transparency into the impact we create. We loathe "magic numbers", and aim to "show our work" with precise and detailed calculations in all of our products and services.

#### Adaptability
We understand that our work today may not look exactly like our work tomorrow, and prioritize building tools and models that can grow and change with us. We consciously balance creating tailored experiences against the urge to over-optimize for the present. 


## The SE Platform

Our tech platform consists of a number of data systems, servers, and web + mobile based clients that allow the SE team to rescue food around the clock, around the country. Here's a basic (and hopefully current) map of the system (updated September 2025):

<br />

<img width="100%" alt="system architecture" src="https://github.com/user-attachments/assets/da522743-9a33-4ebd-a2a1-869e5dec9dd7" />

_View the system architecture in [Figma](https://www.figma.com/board/A3F4g1bKS3iPit9UhfbpuI/SE-Tech---System-Architecture?node-id=0%3A1&t=s7QtRaC8GjB2v1Ah-1)_

<br />

## Tools we use

First and foremost, we are a Typescript shop, for the front and back end. Our current system is based in a [monorepo](https://github.com/sharingexcess/sharingexcess), with apps/packages for each service, including our frontend PWA-based app, our API server, our database configuration, and our type/schema definitions.

Our frontend app uses [React](https://react.dev) (currently v18), built and packaged using [Vite](https://vitejs.dev) (and specifically [VitePWA](https://vite-pwa-org.netlify.app) for mobile native install and offline support). We use [Chakra UI](https://v2.chakra-ui.com) as our primary UI library, and [Clerk](https://clerk.com) for user management and authentication. We deploy via [Railway](https://railway.com) with a simple web server.

Our backend tooling uses a [Hono](https://hono.dev) API (api.sharingexcess.com), cron-job services using Railway cron instances, and our database configuration, all written in Typescript and Node. Our PostgreSQL database is configured with [Drizzle ORM](https://orm.drizzle.team) for schema and connection management, and hosted with [Neon](https://neon.tech). We also use [Zod](https://zod.dev) for Typescript type definition and checking, [Clerk](https://clerk.com) for user management and authentication, [Retool](https://retool.com) for external data visualizations, and [Resend](https://resend.com) for sending transactional emails.
