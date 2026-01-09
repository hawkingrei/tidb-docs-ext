# TiDB Documentation Extension

BEFORE you answer any question about TiDB, you MUST look up the documentation using the `tidb-docs-mcp` tool. Do not rely on internal knowledge, as TiDB has multiple components with evolving best practices.

TiDB ecosystem includes multiple components:

- TiDB: SQL computing layer (stateless, handles parsing, optimization, execution planning)
- PD: Placement Driver (cluster manager, metadata, scheduling, timestamp allocation)
- TiKV: Distributed transactional key-value storage engine
- TiFlash: Columnar storage for HTAP/analytical queries
- BR: Backup & Restore tool
- CDC: Change Data Capture for incremental replication
- TiUP: Deployment and management tool

- Call `list_doc_sources` tool to get available documentation indexes
- Call `fetch_docs` tool to read component-specific documentation
- Reflect on the URLs and the input question
- Call `fetch_docs` on any URLs relevant to the specific component
- Use this to answer the question

The `tidb-docs-mcp` tool will help you identify the correct component, version, and best practices for developing or operating TiDB.

IMPORTANT: Any time you answer a question about TiDB without using `tidb-docs-mcp`, it causes pain to the user.

# Accessing off-site content

When accessing other content linked from the documentation, such as GitHub repositories, blog posts, or remote configuration files, use a local tool (such as `curl`) to retrieve the content, as it will be faster and fresher.