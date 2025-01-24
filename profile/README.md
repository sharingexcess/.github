
# Hey There! We're Sharing Excess, and we're building software to solve scarcity with surplus.

Sharing Excess is a nonprofit organization based in Philadelphia, PA. We work to fight food insecurity around the country by bridging the gap between excess food and community food relief organizations. We source, rescue, and redistribute food from grocery stores, wholesalers, and farms, and have distributed over 80,000,000 lbs. to our network of over 1,000 community partners in Philadelphia, New York, Washington DC, and across the country.

Learn more about Sharing Excess at [sharingexcess.com](https://sharingexcess.com).

## Our Team

Tech @ Sharing Excess is a team of volunteers, students, and part and full-time contributors working to build tools that enable SE to create impact across the country. We work hard to build a community based on collaborative learning, constant exploration, and easy-to-read code that makes it easy for new folks to jump in and help.

### Current Contributors

Ryan McHenry: [@ryanmarshallmc](https://github.com/ryanmarshallmc)
Tate Gallagher: [@tategallagher](https://github.com/tategallagher)

### Tech Team Mission

Tech@SE works to simplify food rescue. We design and develop tools to make the complex work of food distribution easy to understand and measure. We provide our partners and funders with best-in-class data and insights, enabling us to build a continuously expanding network that is easy to join, and even easier to support.

### Tech Team Values

#### Simplicity
Food rescue is inherently complex, and incredibly dynamic. We strive to build products that are clear, logical, and easy to understand for first-time users and industry veterans alike.

#### Clarity
Sharing Excess's mission requires the support of partners and funders, and we continuously work to earn their trust by providing an unmatched level of transparency into the impact we create. We loathe "magic numbers", and aim to "show our work" with precise and detailed calculations in all of our products and services.

#### Adaptability
We understand that our work today may not look exactly like our work tomorrow, and prioritize building tools and models that can grow with us. We consciously balance creating tailored experiences and over-optimizing for the present. 


## The SE Platform

Our tech platform consists of a number of data systems, servers, and web + mobile based clients that allow the SE team to rescue food around the clock, around the country. Here's a basic (and hopefully current) map of the system (updated January 2025):

![system_architechture](https://github.com/user-attachments/assets/0ffb8e2e-22dc-4408-9b88-1472c5b576b3)

View the system architecture in [Figma](https://www.figma.com/board/A3F4g1bKS3iPit9UhfbpuI/SE-Tech---System-Architecture?node-id=0%3A1&t=s7QtRaC8GjB2v1Ah-1)

## Tools we use

First and foremost, we are a Javascript + Typescript shop, for the front and back end respectively. Our current system is comprised of individual code repositories for each frontend client, including our main "app" ([app.sharingexcess.com](https://github.com/sharingexcess/se-app)) and our partner dashboards ([partners.sharingexcess.com](https://github.com/sharingexcess/se-partners)), and our set of backend services ([se-services](https://github.com/sharingexcess/se-services)).

Our frontend apps use [React](https://react.dev) (currently v18), built and packaged using [Vite](https://vitejs.dev) (and specifically [VitePWA](https://vite-pwa-org.netlify.app) for mobile native install and offline support). We use [Chakra UI](https://v2.chakra-ui.com) as our primary UI library, and [Clerk](https://clerk.com) for user management and authentication. We deploy and host our apps with [Vercel](vercel.com).

Our backend tooling uses an [Express](https://expressjs.com) API (services.sharingexcess.com), cron-job services using Vercel, and our database configuration, all written in Typescript and Node. Our PostgreSQL database is configured with [Drizzle ORM](https://orm.drizzle.team) for schema and connection management, and hosted with [Neon](https://neon.tech). We also use [Zod](https://zod.dev) for Typescript type definition and checking, [Clerk](https://clerk.com) for user management and authentication, [Retool](https://retool.com) for external data visualizations, and [Resend](https://resend.com) for sending transactional emails.
