# Typewriter

If we don't skip generation, a CSDL will be generated from the docs. It will describe things that can't be done. Thatis now we generated the AnnotationOptions* metadata. 

## from typewriter

Using the following cmd line:

`-v Info -l CSharp -m D:\repos\MSGraph-SDK-Code-Generator\metadata\2018_10_23\v1.0_2018_10_23_source.xml -o generated123 -d D:\repos\microsoft-graph-docs`

## Using the annotation options

csdlWithDocAnnotations_AnnotationOptions.* files were done with the following options:

            var csdlWriterOptions = new CsdlWriterOptions()
            {
                DocumentationSetPath = options.DocsRoot + "\\api-reference\\v1.0\\",
                Annotations = AnnotationOptions.AllAnnotations,
                MergeWithMetadataPath = options.Metadata,
                SkipMetadataGeneration = true,
                Formats = MetadataFormat.EdmxInput
            };

## Using the no annotation options


csdlWithDocAnnotations_NoAnnotationOptions.xml was done with the following

            var csdlWriterOptions = new CsdlWriterOptions()
            {
                DocumentationSetPath = options.DocsRoot + "\\api-reference\\v1.0\\",
                MergeWithMetadataPath = options.Metadata,
                SkipMetadataGeneration = true,
                Formats = MetadataFormat.EdmxInput
            };

## Older.xml
Used: 

`typewriter.exe -v Info -l CSharp -m D:\repos\MSGraph-SDK-Code-Generator\metadata\2018_09_14\v1.0_2018_09_14_source.xml -o generated -d D:\repos\docs`
 with the following options

             var csdlWriterOptions = new CsdlWriterOptions()
            {
                DocumentationSetPath = options.DocsRoot + "\\api-reference\\v1.0\\",
                MergeWithMetadataPath = options.Metadata,
                SkipMetadataGeneration = true,
                Formats = MetadataFormat.EdmxInput
            };

