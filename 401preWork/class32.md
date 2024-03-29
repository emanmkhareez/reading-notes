Context API - Behaviors
Review, Research, and Discussion
When you have multiple contexts, what component type should you use (class/function) and why?
Class components are ES6 classes and Functional Components are functions. The only constraint for a functional component is to accept props as an argument and return valid JSX.
What are some good use cases for using the Context API for global state?
Ebay : Unlike the previous companies, eBay didn’t start out with the intent of being API-driven.
Twilio : Twilio really defines what it means to be API-driven.
Stripe : Stripe is one of the most successful and best known API-driven businesses.
Salesforce : XML APIs have been a part of Salesforce since day one, back in 2000 when it launched.
How can you best test context?
The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).
Document the following Vocabulary Terms
Context: Context provides a way to pass data through the component tree without having to pass props down manually at every level.
useContext(): is a hook used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.
static context: the static context is used to configure prepare-time characteristics.
Note: Prepare-time refers to the execution of one of the prepare methods on XFactory or the execution of one of the compile methods on XCompilationFactory.
Preparation Materials
context api

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

When to Use Context??

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component.
You can only subscribe to a single context using this API. If you need to read more than one see Consuming Multiple Contexts. If you are using the experimental public class fields syntax, you can use a static class field to initialize your contextType.

API

React.createContext
Context.Provider
Class.contextType
Context.Consumer
Context.displayName