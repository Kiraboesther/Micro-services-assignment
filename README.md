# Microservices: How Companies Use Them and Why Some Moved Away

**Name:** Kirabo Esther Kebirungi  
**Registration Number:** S24B23/045

---

## 1. How Netflix Uses Microservices

Netflix is probably the most well-known example of a company that uses microservices. Before switching to this approach, Netflix ran on one big system. This worked fine at first, but as the number of users grew, problems started coming up. If one part of the system broke down, the whole platform could go offline. So, Netflix decided to break its system into smaller, separate parts called microservices.

Today, Netflix uses hundreds of these small services, and each one handles a specific job. For example, one service manages user logins, another handles video streaming, another deals with recommendations, and so on. These services work independently but still communicate with each other.

Some key ways Netflix uses microservices include:

- **Streaming Service:** Manages video playback and adjusts quality based on the user's internet speed.
- **Recommendation Engine:** Suggests movies and shows based on viewing history.
- **Billing Service:** Handles all payments separately from the rest of the platform.
- **API Gateway:** Acts as a single entry point that directs user requests to the right service.

Because of this setup, if the recommendation service goes down, users can still watch their shows. Netflix also built tools like Chaos Monkey, which randomly shuts down parts of the system on purpose to test how well it handles failures. This approach has helped Netflix grow to serve over 230 million subscribers around the world.

---

## 2. Other Companies That Use Microservices

Many large tech companies have adopted microservices because they need systems that can handle millions of users without crashing. Below are some well-known examples:

### Amazon

Amazon was actually one of the first companies to move to microservices. In the early 2000s, their website ran on one large system that became very difficult to manage. They split it up so that services like product search, cart management, checkout, and payments all run independently. This is why Amazon can handle massive amounts of traffic, especially during events like Black Friday, without the whole site going down.

### Uber

Uber started as a small app but grew very quickly. As they expanded to more cities and countries, their original single system could not keep up. They broke their app into microservices where different parts handle driver matching, fare calculation, GPS tracking, and notifications. Each of these services can be updated or scaled up without touching the others.

### Spotify

Spotify uses microservices to manage its music streaming platform. Their services are split into small teams, where each team owns and maintains a specific service. For example, there are separate services for music playback, playlists, artist pages, and user accounts. This makes it easy for Spotify to release new features without disrupting the rest of the app.

### Airbnb

Airbnb also switched from a single system to microservices as their platform grew. They now have separate services for listings, bookings, payments, and user messaging. This helps them add new features quickly and handle high traffic during popular travel seasons.

---

## 3. Companies That Dropped Microservices and Went Back to Monolithic

While microservices work well for large companies, some businesses have found that they come with too much complexity, especially for smaller teams. A few companies have actually moved away from microservices and gone back to a monolithic system, where everything is in one place.

### What is a Monolithic System?

A monolithic system is the opposite of microservices. Instead of breaking the application into many small parts, everything is built and deployed as one single unit. While this can make things simpler to manage at first, it becomes harder to scale as the application grows. However, for smaller teams, it can actually be easier to work with.

### Stack Overflow

Stack Overflow is a popular website used by millions of developers. Despite its size, it actually runs on a mostly monolithic system. They found that their team was small enough that managing many microservices would have been more trouble than it was worth. Their monolithic setup runs efficiently on just a few servers.

### Basecamp (Hey)

Basecamp, the company behind project management tools like Basecamp and the Hey email service, has spoken openly about choosing a monolithic approach. Their developers argue that microservices add unnecessary complexity for teams that do not actually need them. They believe that a well-built monolithic app is easier to test, deploy, and maintain.

### Segment

Segment is a data analytics company that actually tried microservices and then moved back to a monolithic system. They split their system into over 140 microservices, but this created serious problems. Managing so many services became a full-time job. Communication between services was slow, and it was hard to figure out what was causing bugs. Eventually, they rebuilt everything into one large system and found it much easier to work with.

### Prime Video (Amazon)

Interestingly, even Amazon, which is famous for using microservices, found a case where going back to basics helped. In 2023, the Amazon Prime Video team shared that they moved one of their video monitoring tools from a microservices setup to a monolithic one. The result was that their costs dropped by over 90% and the system became much simpler to manage. This shows that microservices are not always the best choice, even for large companies.

---

## Conclusion

Microservices have changed the way many large companies build and manage their software. Companies like Netflix, Amazon, Uber, and Spotify have benefited from breaking their systems into smaller independent parts that can grow and be updated easily. However, microservices are not perfect for everyone. Smaller teams or companies with less complicated systems may find that a monolithic approach is cheaper, simpler, and easier to manage. The best architecture depends on the size, needs, and resources of the company.
