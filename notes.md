# from typewriter

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

