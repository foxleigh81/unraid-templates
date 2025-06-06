# Unraid Templates

A repository to store Docker container templates for applications published on the Unraid Community Applications store.

## Repository Structure

```plaintext
unraid-templates/
├── foxleigh81/          # Templates by foxleigh81
│   └── strip-ai.xml     # Strip-AI text normalisation tool
└── README.md           # This documentation
```

## Available Templates

### Strip-AI

**File:** `foxleigh81/strip-ai.xml`

A lightweight text normalisation tool that removes AI-generated formatting quirks from text.

**Features:**

- Removes em/en dashes, smart quotes, and extra spaces
- Strips emoji from text (optional)
- Clean, minimal web interface
- Static React application served via nginx

**Docker Details:**

- **Image:** `foxleigh81/strip-ai`
- **Registry:** [Docker Hub](https://hub.docker.com/r/foxleigh81/strip-ai)
- **Project:** [strip-ai.spacenectar.io](https://strip-ai.spacenectar.io)
- **Support:** [GitHub Repository](https://github.com/foxleigh81/strip-ai)
- **Category:** Productivity
- **Web UI Port:** 3000 (maps to container port 80)

**Environment Variables:**

- `NODE_ENV`: Set to `production` (default)

## Usage Instructions

### For Unraid Users

1. Open the Unraid web interface
2. Navigate to **Apps** tab
3. Search for the desired application (e.g., "Strip-AI")
4. Click **Install** and configure as needed
5. Start the container

### Manual Template Installation

If you need to manually add a template:

1. Copy the raw URL of the desired XML template:

   ```plaintext
   https://raw.githubusercontent.com/foxleigh81/unraid-templates/main/foxleigh81/[template-name].xml
   ```

2. In Unraid, go to **Docker** tab
3. Click **Add Container**
4. Set **Template** to the raw GitHub URL
5. Configure and deploy

### Direct Template URLs

- **Strip-AI:** `https://raw.githubusercontent.com/foxleigh81/unraid-templates/main/foxleigh81/strip-ai.xml`

## Template File Structure

Each XML template contains:

- Container metadata (name, description, overview)
- Docker image repository information
- Port mappings and networking configuration
- Environment variables
- Web UI access information
- Support and project links
- Donation information

## Contributing

To add new templates:

1. Create appropriately named XML files following the existing structure
2. Include all required metadata fields
3. Test templates thoroughly before submission
4. Update this README with new template information

## Support

For issues with individual applications, please use the support links provided in each template. For template-specific issues, please open an issue in this repository.

## Donations

If you find these templates useful, consider supporting the maintainer:

- [Ko-fi: foxleigh81](https://ko-fi.com/foxleigh81)
