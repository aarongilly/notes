---
created: 2023-07-08
aliases: 
tags:
  - coding
  - modeling
---
**The set of properties and methods available on an object. **

The term “interface” has a lot of meanings. From a modeling and software perspective, the term refers to a set of properties and methods available on an object. Many languages (such as Java or [[TypeScript]]) have dedicated syntax for declaring interfaces and semantics for using them.

Example from my [[PDW]] :

```tsx
/**
 * The `DataStore` interface is what you must implement when creating code to
 * hook up a new database. It is what sits between the data store of choice and the PDW.
 * It's designed to be as simple-to-implement as possible.
 * 
 * The parameter sanitization & merge logic are handled by the PDW.
 * 
 * It's *very much* a work in progress.
 */
export interface DataStore {

    getDefs(params: SanitizedParams): DefLike[];

    getEntries(params: SanitizedParams): EntryLike[];

    getTags(params: SanitizedParams): TagLike[];

    setDefs(defs: Def[]): Def[];

    setEntries(entries: Entry[]): Entry[];

    setTags(tagData: Tag[]): TagLike[];

    query(params: QueryParams): QueryResponse;

    getOverview(): DataStoreOverview;

    connect?(...params: any): boolean;

    /**
     * The name of the connector, essentially. Examples: "Excel", "Firestore"
     */
    serviceName: string;

    /**
     * A reference to the Personal Data Warehouse instance to 
     * which the storage connector is connected.
     */
    pdw: PDW;
}
```

****
### Source

Mostly myself, but also I liked this:

[What is the definition of "interface" in object oriented programming](https://stackoverflow.com/questions/2866987/what-is-the-definition-of-interface-in-object-oriented-programming)

### Related
- [[UML Components]]