This repository demonstrates a subtle bug in React Router Dom v6 related to route matching with dynamic segments.  When a route with a dynamic segment is not found, the root route ('/') unexpectedly matches instead of the 404 route. The solution provides a fix for the issue by ensuring the catch-all route ('*') takes precedence over the root route.