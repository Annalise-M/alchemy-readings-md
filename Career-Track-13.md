<a href="https://docs.mongodb.com/manual/core/aggregation-pipeline/">Mongo Aggregations</a>

<a href="https://www.compose.com/articles/aggregations-in-mongodb-by-example/">Aggregations by Example</a>

---
    Mongo Aggregations -
        The aggregation pipeline is a framework for data aggregation modeled on the concept of data processing pipelines. Documents enter a multi-stage pipeline that transforms the documents into aggregated results.
    
<img src="ct-mongo-aggregation-ref" />

    Pipeline

        The MongoDB aggregation pipeline consists of stages. Each stage transforms the documents as they pass through the pipeline. Pipeline stages do not need to produce one output document for every input document; e.g., some stages may generate new documents or filter out documents.

    Pipeline stages can appear multiple times in the pipeline with the exception of $out, $merge, and $geoNear stages. 

    
Go to <a href="https://docs.mongodb.com/manual/reference/operator/aggregation-pipeline/#aggregation-pipeline-operator-reference">Aggregation Pipeline Stages</a> for a list of all available stages.

    Pipeline Expressions - 
        Some pipeline stages take a pipeline expression as the operand. Pipeline expressions specify the transformation to apply to the input documents. Expressions have a document structure and can contain other expression.

        Pipeline expressions can only operate on the current document in the pipeline and cannot refer to data from other documents: expression operations provide in-memory transformation of documents.


    Pipeline Operators and Indexes -
        MongoDB’s query planner analyzes an aggregation pipeline to determine whether indexes can be used to improve pipeline performance.

        $match:
            The $match stage can use an index to filter documents if it occurs at the beginning of a pipeline.

        $sort:
            The $sort stage can use an index as long as it is not preceded by a $project, $unwind, or $group stage.
        
        $group:
            The $group stage can sometimes use an index to find the first document in each group if all of the following criteria are met:

                - The $group stage is preceded by a $sort stage that sorts the field to group by,
                - There is an index on the grouped field which matches the sort order and
                - The only accumulator used in the $group stage is $first.

        See Optimization to Return the First Document of Each Group for an example.

        $geoNear
        The $geoNear pipeline operator takes advantage of a geospatial index. When using $geoNear, the $geoNear pipeline operation must appear as the first stage in an aggregation pipeline.

___
    Aggregations by Example -

        The aggregate function accepts an array of data transformations which are applied to the data in the order they're defined. This makes aggregation a lot like other data flow pipelines: the transformations that are defined first will be executed first and the result will be used by the next transformation in the sequence.

        The first stage of the pipeline is matching, and that allows us to filter out documents so that we're only manipulating the documents we care about. The matching expression looks and acts much like the MongoDB find function or a SQL WHERE clause.

            (for more, see link)


