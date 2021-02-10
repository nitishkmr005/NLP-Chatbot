# NLP-Loading Reddit data

Reddit data -
---------------

The structure of Reddit is in a tree-form, not like a forum or something where everything is linear. The parent comments are linear, but replies to parent comments branch out.

-Top level reply 1
--Reply to top level reply 1
--Reply to top level reply 1
---Reply to reply...
-Top level reply 2
--Reply to top level reply 1
-Top level reply 3
The structure we need for deep learning is input-output. So we really are trying to get something more along the lines of comment and reply pairs. In the above example, we could use the following as comment-reply pairs:

-Top level reply 1 and --Reply to top level reply 1
