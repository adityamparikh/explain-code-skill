# Java/Spring Boot Equivalents

## What to Map

| Foreign Concept | Map To |
|---|---|
| **Language constructs** | Java or Kotlin equivalent syntax, idioms, and types |
| **Build system** (npm, pip, cargo, go mod, etc.) | Maven or Gradle equivalent (dependencies, plugins, tasks) |
| **Web framework** (Express, Flask, Django, Gin, Actix, etc.) | Spring MVC / Spring WebFlux equivalent (controllers, filters, interceptors) |
| **Dependency injection** (Guice, Dagger, Wire, etc.) | Spring DI (`@Component`, `@Service`, `@Autowired`, constructor injection) |
| **ORM / data access** (SQLAlchemy, TypeORM, GORM, Diesel, etc.) | Spring Data JPA / JdbcTemplate equivalent |
| **Configuration** (.env, TOML, YAML loaders, etc.) | `application.properties` / `application.yml` with `@ConfigurationProperties` |
| **Middleware / filters** | Spring `Filter`, `HandlerInterceptor`, or `@ControllerAdvice` |
| **Testing** (pytest, Jest, Go testing, etc.) | JUnit 5 + Mockito + Spring Boot Test equivalent |
| **Project structure** | Standard Maven/Gradle project layout (`src/main/java`, `src/test/java`) |
| **Package management** | Maven Central / Gradle dependency declarations |
| **CLI / task runners** (Makefile, npm scripts, rake, etc.) | Maven plugins / Gradle tasks |

## Format

Include a subsection like this in the explanation when the code is not Java/Kotlin + Spring Boot:

```
### Spring Boot Equivalent
- **Framework:** [e.g., "Express.js `app.get('/users', handler)` is like a `@GetMapping("/users")` in a `@RestController`"]
- **Build:** [e.g., "`package.json` dependencies are like `<dependency>` entries in `pom.xml`"]
- **Pattern:** [e.g., "This middleware chain works like a Spring `FilterChain`"]
- **Code:** [short Java/Kotlin snippet showing the equivalent approach]
```

