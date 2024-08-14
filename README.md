# MongoDB Methods, Comparison Operators, Logical Operators, Update Operators, Sorting Methods, Aggregation Methods, Indexing Methods, and ACID Transactions Methods

MongoDB methods, comparison operators, logical operators, update operators, sorting methods, aggregation methods, indexing methods, and ACID transactions methods.

## Methods

### aggregate

- **Description**: Performs complex data processing on documents.

### countDocuments

- **Description**: Counts how many documents match a query.

### createIndex

- **Description**: Creates an index to make queries faster.

### delete

- **Description**: Removes documents that match a query.

### deleteAll

- **Description**: Removes all documents from a collection.

### deleteMany

- **Description**: Removes all documents that match a query.

### deleteOne

- **Description**: Removes the first document that matches a query.

### distinct

- **Description**: Finds unique values for a specified field across documents.

### drop

- **Description**: Deletes an entire collection of documents.

### dropIndex

- **Description**: Removes an index from a collection.

### find

- **Description**: Retrieves documents that match a query.

### findOne

- **Description**: Retrieves the first document that matches a query.

### findAndModify

- **Description**: Finds a document and modifies it in one step.

### findOneAndDelete

- **Description**: Finds a document and deletes it in one step.

### findOneAndUpdate

- **Description**: Finds a document and updates it in one step.

### insertMany

- **Description**: Adds multiple documents to the collection at once.

### insertOne

- **Description**: Adds one document to the collection.

### limit

- **Description**: Limits the number of documents returned by a query.

### renameCollection

- **Description**: Changes the name of a collection.

### replaceOne

- **Description**: Replaces the first document that matches a query with a new document.

### skip

- **Description**: Skips a specified number of documents in the query result.

### sort

- **Description**: Arranges documents in a specific order based on a field.

### updateMany

- **Description**: Updates all documents that match a query with new data.

### updateOne

- **Description**: Updates the first document that matches a query with new data.

## ACID Transactions Methods

### startSession

- **Description**: Starts a new session for performing operations in a transaction.

### startTransaction

- **Description**: Starts a transaction within a session.

### commitTransaction

- **Description**: Commits the current transaction, applying all changes.

### abortTransaction

- **Description**: Aborts the current transaction, discarding all changes.

### withTransaction

- **Description**: Executes a series of operations within a transaction, ensuring ACID properties.

## Aggregation Methods

### $addFields

- **Description**: Adds new fields to documents in the aggregation pipeline.

### $bucket

- **Description**: Categorizes documents into groups, called buckets, based on a specified expression.

### $bucketAuto

- **Description**: Automatically categorizes documents into a specified number of buckets based on a specified expression.

### $count

- **Description**: Counts the number of documents in the aggregation pipeline.

### $facet

- **Description**: Allows multiple aggregation pipelines to be run within a single stage on the same set of documents.

### $geoNear

- **Description**: Filters documents by proximity to a specified point and sorts by distance.

### $group

- **Description**: Groups documents by a specified expression and applies an accumulator, like `sum`, to group values.

### $limit

- **Description**: Limits the number of documents passed to the next stage in the pipeline.

### $lookup

- **Description**: Performs a join operation to combine data from two collections.

### $match

- **Description**: Filters documents in the aggregation pipeline to pass only those that match the specified condition.

### $out

- **Description**: Writes the results of the aggregation pipeline to a specified collection.

### $project

- **Description**: Reshapes each document in the aggregation pipeline by adding, removing, or modifying fields.

### $redact

- **Description**: Restricts the content of documents based on information contained in the documents themselves.

### $replaceRoot

- **Description**: Replaces the input document with the specified document.

### $replaceWith

- **Description**: Replaces the input document with the specified document (alias for `$replaceRoot`).

### $sample

- **Description**: Randomly selects the specified number of documents from the input documents.

### $set

- **Description**: Adds new fields or updates existing fields in the input documents (alias for `$addFields`).

### $skip

- **Description**: Skips a specified number of documents in the aggregation pipeline.

### $sort

- **Description**: Sorts the documents in the aggregation pipeline.

### $unwind

- **Description**: Deconstructs an array field from the input documents to output a document for each element.

## Comparison Operators

### $eq (Equal)

- **Description**: Finds documents where the value of a field is exactly equal to the specified value.

### $gt (Greater Than)

- **Description**: Finds documents where the value of a field is greater than the specified value.

### $gte (Greater Than or Equal)

- **Description**: Finds documents where the value of a field is greater than or equal to the specified value.

### $in (In)

- **Description**: Finds documents where the value of a field matches any value in a specified list.

### $lt (Less Than)

- **Description**: Finds documents where the value of a field is less than the specified value.

### $lte (Less Than or Equal)

- **Description**: Finds documents where the value of a field is less than or equal to the specified value.

### $ne (Not Equal)

- **Description**: Finds documents where the value of a field is not equal to the specified value.

### $nin (Not In)

- **Description**: Finds documents where the value of a field does not match any value in a specified list.

## Indexing Methods

### createIndex

- **Description**: Creates an index to make queries faster.

### dropIndex

- **Description**: Removes an index from a collection.

### ensureIndex

- **Description**: Deprecated method to create an index if it does not already exist.

### find

- **Description**: Supports the use of indexes for faster retrieval of documents.

### getIndexes

- **Description**: Returns a list of all indexes on a collection.

### reIndex

- **Description**: Rebuilds all indexes on a collection.

## Logical Operators

### $and (Logical AND)

- **Description**: Matches documents that meet all the specified conditions.

### $nor (Logical NOR)

- **Description**: Matches documents that do not meet any of the specified conditions.

### $not (Logical NOT)

- **Description**: Inverts the effect of a query condition.

### $or (Logical OR)

- **Description**: Matches documents that meet at least one of the specified conditions.

## Update Operators

### $addToSet

- **Description**: Adds a value to an array field only if it doesn't already exist.

### $currentDate

- **Description**: Sets the value of a field to the current date and time.

### $each

- **Description**: Adds each value in a list to an array (often used with `$push`).

### $inc

- **Description**: Increases or decreases the value of a field by a specified amount.

### $max

- **Description**: Updates the value of a field to a specified value if it is greater than the current value.

### $min

- **Description**: Updates the value of a field to a specified value if it is less than the current value.

### $mul

- **Description**: Multiplies the value of a field by a specified number.

### $pop

- **Description**: Removes the first or last item from an array.

### $pull

- **Description**: Removes all instances of a value from an array.

### $pullAll

- **Description**: Removes multiple specified values from an array.

### $push

- **Description**: Adds a value to an array field.

### $rename

- **Description**: Renames a field in a document.

### $set

- **Description**: Sets the value of a field in a document.

### $unset

- **Description**: Removes a field from a document.

### upsert

- **Description**: Adds a document if no matching document is found; otherwise, updates the existing document.

## Sorting Results Methods

### collation

- **Description**: Specifies language-specific rules for string comparison, including sorting.

### sort

- **Description**: Sorts the query results based on one or more fields.
