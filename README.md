# SQLDesk - SQL Query Runner

**Web App’s Link:[https://sqldesk.netlify.app/]**

## Overview

Users can enter SQL queries and view the results of such queries using the web-based SQL editor SQLDESK. In response to the queries, the application shows a table with fictitious data and has a place for entering SQL commands. It gives data analysts an easy-to-use interface so they can work effectively. Because React with Vite is quick, light, and user-friendly, it was used to build the SQL editor. A few other packages are included in the project for improved functionality.


## Packages

- [Material UI](https://mui.com/)
- [react-ace](https://www.npmjs.com/package/react-ace)
- [openai](https://www.npmjs.com/package/openai)
- [axios](https://www.npmjs.com/package/axios)
- [react-router-dom](https://www.npmjs.com/package/react-router-dom)
- [uuid](https://www.npmjs.com/package/uuid)

## Features

- ** AI-Powered Chatbot Assistant:** An intelligent chatbot built to expedite the development of SQL queries is included into SQLDESK.  The chatbot uses the application's dummy datasets to assess user inputs in real time and provide rapid fixes, grammar corrections, and context-aware suggestions.  By eliminating uncertainty and guaranteeing smooth query development, the AI assistant speeds up your process, whether you're debugging a complicated JOIN or optimizing a WHERE clause.
- **Multi-Workspace Architecture:** With the workspace concept in SQLDESK, you can easily organize your tasks.  Assure clear job separation by creating environments specifically for different datasets, teams, or workflows.  In addition to increasing individual productivity, this capability sets the stage for future collaboration solutions by allowing teams to work concurrently without interfering with SQL scripts or results.
- **Multi-Tab Query Editor:** Use the tabbed interface of SQLDESK to do away with context-switching.  You can compare results, iterate on scripts, or test different strategies side by side by opening and managing many SQL queries at once in a same workspace.  For optimal flexibility, each tab functions independently while maintaining execution history and unsaved changes.
- ** Built-In SQL Cheatsheet:** Use a carefully selected library of pre-written SQL snippets to expedite your development.  The cheatsheet offers quick access to syntax examples and best practices for everything from simple SELECT statements to sophisticated window functions.  To locate the ideal template for your requirements, filter by use case (such as data aggregation or table joins).


## Load Time

The Lighthouse Tool, a powerful performance measurement tool that assesses web page loading speed and offers useful insights for optimization, has been used to measure page load time.  With the use of this data, QueryWiz guarantees a flawless user experience with quick loading times for increased satisfaction and productivity.


![Alt text]([https://imgur.com/a/Sy5ObZ8])


## Technical Optimizations in SQLDESK

- **Vite's Built-in Tree Shaking:**During the build process, Vite automatically shakes the tree to remove dependencies and unnecessary code from the finished bundle.  Because only the essential portions of the code are included in the production version, this optimization results in reduced bundle sizes and quicker SQLDESK load times. The Lighthouse Tool, a powerful performance measurement tool that assesses web page loading speed and offers useful insights for optimization, has been used to measure page load time.  With the use of this data, QueryWiz guarantees a flawless user experience with quick loading times for increased satisfaction and productivity.
- **Utilizing useCallback and useMemo Hooks:** useCallback Stabilizes event handlers (query execution, workspace/tab switches) to prevent unnecessary re-renders.
useMemo Memoizes heavy tasks like parsing large datasets (~10k rows) and caching query results for instant reuse.
Result - Smoother UI interactions and faster responses during complex operations.
- **Implementation of Lazy Loading:** Lazy loading is a technique used by SQLDESK to postpone non-essential elements (like the React-ace editor) until they are needed.  The initial bundle size is decreased by dynamically importing these components, guaranteeing better performance and quicker page loads.  For example, there is no upfront resource overhead because the code editor only loads when the user interacts with the query field.

