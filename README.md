# Adaption Plugin for ChatGPT & Codex

Connect ChatGPT and Codex to [Adaption](https://adaptionlabs.ai) for dataset management, fine-tuning, and AutoScientist workflows.

## Installation

### From Plugins Directory (Coming Soon)

1. Open ChatGPT or Codex
2. Go to **Plugins Directory**
3. Search for **"Adaption"**
4. Click **Install**
5. Authenticate with your Adaption account

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/adaptionlabs/adaption-codex-plugin.git
   ```

2. Enable Developer Mode in ChatGPT:
   - Open **Settings** → **Security and login**
   - Turn on **Developer mode**

3. Register the MCP server:
   - Go to **ChatGPT Plugins** → click **+**
   - Enter MCP server URL: `https://api.adaption.ai/api/v1/mcp`
   - Complete authentication

4. Add to local marketplace (optional):
   - Use `@plugin-creator` or manually create a marketplace entry
   - Point to the cloned plugin directory

### Get Your API Key

1. Go to [app.adaptionlabs.ai/settings/api-keys](https://app.adaptionlabs.ai/settings/api-keys)
2. Create a new API key
3. Use it when authenticating the MCP server connection

## Features

### 📊 Dataset Management (11 tools)

- **Import** datasets from HuggingFace, Kaggle, or Google Sheets
- **Adapt** datasets with Adaption's processing pipeline
- **Augment** datasets with synthetic domain/general rows
- **Translate** and **localize** dataset content
- **Combine** multiple datasets
- **Export** processed results

### 🎯 Fine-tuning (5 tools)

- Browse available **base models**
- Get **hyperparameter recommendations**
- Launch **AutoScientist training runs**
- Monitor **training progress** and results

### 🔬 Invent (2 tools)

- Explore available **domains and subdomains**
- **Generate synthetic datasets** from natural language descriptions

## Available Skills

| Skill | Description |
|-------|-------------|
| `adaption-dataset` | Dataset import, processing, and transformation workflows |
| `adaption-training` | AutoScientist training run management |
| `adaption-invent` | Synthetic data generation with Invent |

## MCP Tools Reference

### Dataset Tools

| Tool | Description |
|------|-------------|
| `list_datasets` | List datasets visible to your organization |
| `get_dataset` | Get details of one dataset |
| `get_dataset_status` | Poll processing status and progress |
| `get_dataset_evaluation` | Get quality evaluation results |
| `get_dataset_export_links` | Get export download URLs |
| `import_dataset` | Import from HuggingFace, Kaggle, or Google Sheets |
| `run_dataset_adaptation` | Estimate or launch adaptation |
| `augment_dataset` | Add synthetic domain/general rows |
| `translate_dataset` | Translate rows to target languages |
| `localize_dataset` | Localize for country/language pairs |
| `combine_datasets` | Combine compatible datasets |

### Training Tools

| Tool | Description |
|------|-------------|
| `list_training_models` | List available base models |
| `list_autoscientist_runs` | List training runs |
| `get_autoscientist_run` | Get run details and progress |
| `recommend_autoscientist_hyperparameters` | Get recommended config |
| `create_autoscientist_run` | Launch training (spends credits) |

### Invent Tools

| Tool | Description |
|------|-------------|
| `list_invent_domains` | List valid domain/subdomain codes |
| `generate_dataset` | Estimate or launch dataset generation |

## Example Usage

Once installed, interact with Adaption through natural conversation:

> "List my Adaption datasets"

> "Import this HuggingFace dataset and adapt it for fine-tuning"

> "Start fine-tuning on my adapted dataset and pick a suitable base model"

> "Generate 1000 customer service examples using Invent"

> "Check the status of my training job"

## Requirements

- ChatGPT Plus or Codex subscription
- Adaption account with API access
- API key with MCP scopes

## Support

- **Documentation**: [docs.adaptionlabs.ai](https://docs.adaptionlabs.ai)
- **Issues**: [GitHub Issues](https://github.com/adaptionlabs/adaption-codex-plugin/issues)
- **Email**: support@adaptionlabs.ai

## License

MIT License - see [LICENSE](LICENSE) for details.
