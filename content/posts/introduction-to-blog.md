+++
title = 'Introduction to Blog'
date = 2024-09-30T23:29:43+08:00
draft = false
+++
# introduction to blog
## Introduction

This website is a blog and archive site of Pleuston. You can find all published documents and communications on this site, including but not limited to:
1. Files
2. Public Communications
3. Published Articles
4. Drafts
5. Blogs

Some content may be encrypted or published in encrypted form, but the article itself will still be published in full as required by regulations.

## Some Regulations

```
...

Pleuston uses a custom archive format to store files and documents. According to the regulations, all the files and documents has to be stored and published.

however, due to the "Document Security Policy", some of the files may be encrypted, the author or the sender has the right to decide which parts of the document should be encrypted and which parts should not.

...

## Regulations

### The Green Shade Capital Information Policy

...

For any unofficial project in the following stages: project operation, project suspension, or project interruption, all the generated documents need to be made public and the blockchain maintained.

Generally speaking, files can be stored in plain text format, and the following issues need to be noted:
1. Line break issues: both LF or CRLF line breaks are supported.
2. Regular expression issues: Metadata needs to be in a clear and consistent format to ensure that regular expressions can accurately and unambiguously identify the target information.
3. Metadata issues: All the metadata are order-independent, for multi-words metadata name, use HTTP Header like format to separate the words. For example, "Author" can be "Author: John Doe" or "Author: John_Doe". "CoAuthor" can be "Co-Author: Jane Smith" or "Co-Author: Jane_Smith".
4. Encryption issues: if the file is encrypted, the id of the file should be published in the metadata. For pure text file, PGP encryption is recommended. For binary file, please refer to the relevant requirements below.

If the file cannot represent by plain text format, files stored in binary format are still supported.

Regardless of the original format of the file, only two forms are allowed for binary files for storage: PDF file form and compressed volume sequence group form.

Both binary original versions or distributed versions of these two file formats participate in blockchain calculations. If the distributed version of the file wants to participate in blockchain calculations, it is necessary to ensure that the file hash of the distributed version is consistent with the original version. The technical department does not recommend using the distributed version to replace the original version, because some operating systems or file systems may embed metadata into the file content, resulting in inconsistent calculated hashes, thereby destroying the stability of the blockchain. 

There are five types of text files have to maintain the File Blockchain:

Articles, Drafts, Proposals, Documents, Communications.

For Articles, An Article is a written work that is published by an individual or an organization. Following meta information has to be maintained:
Title, Authors, Date of Publications, Date of Completion, Keywords, Body.
...

```

We have not yet decided how to use these inherent criteria.