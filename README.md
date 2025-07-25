# n8n-databricks-workflows

This repository contains example workflows and agents that use Databricks features in n8n. These templates demonstrate how to integrate Databricks capabilities like Unity Catalog, Databricks SQL, and Model Serving, and Databricks chat models with n8n workflows.

## 📁 Repository Structure & Templates

### 🤖 Agents
Multi-agent workflows that leverage Databricks capabilities:

#### ✅ Customer support multi-agent.json
- **Purpose**: Automated customer support with Databricks knowledge base
- **Features**: Multi-agent conversation, knowledge retrieval, ticket management
- **Use Cases**: Customer service automation, FAQ handling

#### ✅ Databricks Apps Knowledge Assistant.json
- **Purpose**: AI-powered assistant for Databricks Apps documentation
- **Features**: Knowledge base querying, context-aware responses
- **Use Cases**: Developer support, documentation assistance

#### ✅ Sales Genie multi-agent.json
- **Purpose**: Sales process automation with predictive analytics
- **Features**: Lead scoring, opportunity tracking, sales forecasting
- **Use Cases**: Sales automation, CRM integration

#### 🤖 Genie.json
- **Purpose**: General-purpose Databricks agent
- **Features**: Versatile AI agent for various Databricks tasks
- **Use Cases**: General automation, task assistance

#### 🤖 Next Best Action.json
- **Purpose**: Predictive analytics workflow
- **Features**: ML model integration, recommendation engine
- **Use Cases**: Predictive analytics, decision support

### 🔄 Workflows
Single-purpose workflows for specific Databricks use cases:

#### ✅ Databricks news social media post generator.json
- **Purpose**: Automated content creation from Databricks news
- **Features**: News aggregation, content generation, social media posting
- **Use Cases**: Marketing automation, content marketing

#### ✅ Scrape docs to volumes.json
- **Purpose**: Document processing and storage in Databricks Volumes
- **Features**: Web scraping, document parsing, Unity Catalog integration
- **Use Cases**: Data ingestion, document management

## 🚀 How to Use These Templates

### Method 1: Direct Import (Recommended)

1. **Download the JSON file** from this repository
2. **In n8n:**
   - Go to your n8n instance
   - Click "Import from file" or "Import from URL"
   - Select the downloaded JSON file
   - The workflow will be imported with all nodes and configurations

### Method 2: Copy and Paste JSON

1. **Open the JSON file** in this repository
2. **Copy the entire JSON content**
3. **In n8n:**
   - Create a new workflow
   - Click the three dots menu (⋮) in the top right
   - Select "Import from JSON"
   - Paste the copied JSON content
   - Click "Import"

### Method 3: Import from URL

1. **Get the raw URL** of the JSON file from GitHub
   - Click on any JSON file in this repository
   - Click the "Raw" button
   - Copy the URL
2. **In n8n:**
   - Use "Import from URL" option
   - Paste the raw GitHub URL
   - The workflow will be imported automatically

## ⚙️ Configuration Requirements

### Prerequisites
- n8n instance (self-hosted or cloud)
- Databricks workspace access
- Databricks SQL warehouse
- Unity Catalog setup (for some workflows)

### Required Credentials
Most workflows require these Databricks credentials:
- **Databricks Host**: Your Databricks workspace URL
- **Access Token**: Personal access token from Databricks
- **SQL Warehouse ID**: For SQL queries

## 🔧 Customization

### Before Running
1. **Update credentials** in each workflow node
2. **Modify SQL queries** to match your schema
3. **Adjust parameters** for your specific use case
4. **Test with small datasets** first

## 🛠️ Troubleshooting

### Common Issues
1. **Authentication errors**: Verify Databricks credentials
2. **SQL errors**: Check warehouse status and permissions
3. **Import failures**: Ensure JSON is valid and complete
4. **Node errors**: Verify all required parameters are set

### Getting Help
- Check the n8n documentation for Databricks nodes
- Review Databricks API documentation
- Test individual nodes before running full workflows

## 🤝 Contributing

To add your own workflows:
1. Create a new JSON file in the appropriate directory
2. Use descriptive naming with emojis for status
3. Include comprehensive documentation in the workflow description
4. Test thoroughly before submitting

---

**Note**: These templates are examples and may require customization for your specific environment and use cases. Always test in a development environment before deploying to production.
