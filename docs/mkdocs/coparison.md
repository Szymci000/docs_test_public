## Comparison Table

| Feature / Criteria | **MkDocs** | **Docusaurus** | **Wiki.js** | **WordPress** |
|--------------------|------------|----------------|-------------|----------------|
| Type | Static Site Generator | Static Site Generator (React & MDX) | Dynamic Wiki | CMS (Blog/Pages) |
| **Markdown First** | ✔️ 100% Markdown | ✔️ Markdown + MDX | ✔️ Markdown (DB-backed) | Partial (via plugin) |
| Editing Experience | File-based | File-based (MDX) | Browser editor + Markdown | Browser editor (rich text) + Markdown (plugins) |
| Self-Hosting | ✔️ Simple | ✔️ Simple | ✔️ Requires app + DB | ✔️ PHP + MySQL |
| Installation Complexity | Low | Medium (Node) | Medium (Node + DB) | Medium (PHP stack) |
| Search | Built-in (Lunr/Algolia) | Built-in (Local/Algolia) | Full-text search | Plugin-dependent |
| Navigation / Sidebar | Auto / Manual | Manual + Config | Dynamic trees | Menu system |
| Versioning Support | Via config | Built-in versioning | Not native (via pages) | Plugin / workflow |
| Role/Permission Controls | Git + build workflow | Git + build workflow | Built-in RBAC | Built-in user roles |
| Live Editing | No | No | Yes | Yes |
| Media Handling | File assets | File assets | Attachments | Media Library |
| Plugin Ecosystem | Good | Good | Growing | Very Large |
| Extensible via Plugins | ✔️ | ✔️ | ✔️ | ✔️ |
| Performance | Very Fast (static) | Very Fast (static) | Depends on server | Depends on server |
| Git Integration | Native (files) | Native (files) | Optional | Via plugins |
| Best For | Developer docs, static sites | Versioned docs, interactive docs | Team wiki, knowledge base | Content sites + docs/blog hybrid |
| Markdown Output | Source is Markdown | Source is Markdown/MDX | Stores Markdown in DB or file | Not native Markdown |
| CI/CD Friendly | Excellent | Excellent | Good | Good (with plugins) |
| AI / Indexing Friendly | Excellent (flat files) | Excellent (flat files) | Good (DB + files) | Depends on export |

## Summary

### **MkDocs**
- **Strengths:** Extremely simple static docs, flat Markdown workflow, fast publishing.
- **Considerations:** No live browser editing; file-based workflow required.

### **Docusaurus**
- **Strengths:** Modern React features, versioning, strong for technical docs with UI elements.
- **Considerations:** Requires Node.js environment; MDX learning curve.

### **Wiki.js**
- **Strengths:** True collaborative wiki with browser editing, structured search, RBAC.
- **Considerations:** Requires a database and server environment.

### **WordPress**
- **Strengths:** Very flexible CMS, huge plugin ecosystem, strong WYSIWYG editing.
- **Considerations:** Markdown is not native; needs plugins for export and Markdown workflows.

---

## Recommendation Notes

- **For Markdown-centric documentation with a Git workflow:** *MkDocs* or *Docusaurus* are ideal.
- **For team knowledge base with live editing and access control:** *Wiki.js* is the best fit.
- **For mixed content (blog + docs) with a rich plugin ecosystem:** *WordPress* works but may need add-ons.

---