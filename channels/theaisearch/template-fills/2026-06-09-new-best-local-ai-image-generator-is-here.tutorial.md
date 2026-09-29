---
video_id: OA4gchz1Zcs
template_id: tutorial
template_version: 1
source_summary: ../summaries/2026-06-09-new-best-local-ai-image-generator-is-here.md
source_transcript: ../transcripts/2026-06-09-new-best-local-ai-image-generator-is-here.md
source_summary_hash: sha256:eacbee5caee7741a05b77fe9571124467c413d36ec61959315c41704086c0308
source_transcript_hash: sha256:465bece7aba487e40a437dda1138d98e94230b0748b5a3d7bf329cca724dc190
fill_id: e842c326-5f43-44af-9798-34f2a664d573
published_at: '2026-06-10T09:24:27.568588'
key_points_suppressed: true
provenance: agent:template-fill-v1
---

## Headline takeaway

Install Ideogram 4 in Comfy UI with bounding box controls for precise, high-quality local image generation.

## Prerequisites

### Comfy UI
- **Kind**: tool
- **Note**: Popular platform for running open-source image generators offline with automatic CPU offloading.

### Comfy UI Manager
- **Kind**: tool
- **Note**: Required to detect and install missing nodes for the workflow.

### Ideogram 4 Models
- **Kind**: tool
- **Note**: Main diffusion model, unconditional model, and clip text encoder (FP8 or NVFP4).

### Flux 2 VAE
- **Kind**: tool
- **Note**: Required VAE file for the workflow, approx 336 MB.

### KJ Nodes
- **Kind**: tool
- **Note**: GitHub repository for the KJ prompt builder node if not installed via manager.

### Git
- **Kind**: tool
- **Note**: Required to clone the KJ Nodes repository into the custom nodes folder.

## Steps

### Download and load the workflow
- **Timestamp**: [09:23](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=563)
- **Action**: Download the recommended workflow file from the description and drag it into the Comfy UI interface.
- **Command Or Clicks**: File > Download (from description link) > Drag and drop onto interface
- **Choice Branch**: Use the recommended KJ prompt builder workflow instead of the error-prone JSON template.

### Install Comfy UI Manager
- **Timestamp**: [13:13](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=793)
- **Action**: Open command prompt in the root Comfy UI folder and run the installation script for the manager.
- **Command Or Clicks**: cmd > paste installation script > save run.bat with --enable-manager > restart
- **Choice Branch**: Use the Windows portable version as recommended.

### Install missing nodes via Manager
- **Timestamp**: [13:13](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=793)
- **Action**: Open the Manager, go to Missing Nodes, and install all listed nodes.
- **Command Or Clicks**: Manager > Missing Nodes > Install for all > Apply Changes > Restart
- **Choice Branch**: Restart Comfy UI after applying changes.

### Manually install KJ Nodes if missing
- **Timestamp**: [14:01](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=841)
- **Action**: If the KJ prompt builder is still missing, clone its GitHub repo into the custom_nodes folder.
- **Command Or Clicks**: cd custom_nodes > git clone <repo_url>
- **Choice Branch**: Use git pull to update if already installed.

### Download and place Ideogram 4 models
- **Timestamp**: [16:07](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=967)
- **Action**: Download the main IOG 4 model, unconditional model, and clip text encoder (FP8 recommended) from the linked page.
- **Command Or Clicks**: Download FP8 versions > Save to models/diffusion_models and models/text_encoders
- **Choice Branch**: Ensure both main and unconditional models are downloaded.

### Download and place Flux 2 VAE
- **Timestamp**: [17:02](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1022)
- **Action**: Download the Flux 2 VAE file and place it in the VAE models folder.
- **Command Or Clicks**: Download Flux 2 VAE > Save to models/VAE
- **Choice Branch**: Refresh model list with 'R' after each download.

### Configure workflow nodes
- **Timestamp**: [17:02](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1022)
- **Action**: Select the downloaded models in the respective dropdowns for the diffusion model, text encoder, and VAE.
- **Command Or Clicks**: Select models in dropdowns > Red outlines should disappear
- **Choice Branch**: Ensure no red error outlines remain.

### Set aspect ratio and prompt
- **Timestamp**: [18:50](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1130)
- **Action**: Set the megapixels/aspect ratio and enter the high-level description in the prompt builder.
- **Command Or Clicks**: Set aspect ratio (e.g., 3:4) > Enter description in Ideogram prompt builder
- **Choice Branch**: Specify style, aesthetics, lighting, and medium parameters.

### Draw bounding boxes for elements
- **Timestamp**: [20:02](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1202)
- **Action**: Draw bounding boxes on the canvas for each object in the prompt to bypass the safety filter.
- **Command Or Clicks**: Drag boxes on canvas > Type object description in each box
- **Choice Branch**: Must draw boxes to generate; text-only prompts trigger safety filters.

### Generate and refine images
- **Timestamp**: [25:48](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1548)
- **Action**: Press run to generate. Use 'Grab Background' to reposition elements while keeping the seed fixed.
- **Command Or Clicks**: Press Run > Grab Background > Adjust boxes > Press Run again
- **Choice Branch**: Use 'New Fixed Random' to shuffle seed for variations.

## Gotchas

### Text-only prompts trigger a safety filter image; you must draw bounding boxes to generate content.
- **Severity**: blocking
- **Timestamp**: [18:50](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1130)

### The original V4 workflow requires error-prone JSON formatting; use the KJ prompt builder workflow instead.
- **Severity**: serious
- **Timestamp**: [09:23](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=563)

### Ideogram 4 has a non-commercial license; commercial use requires contacting sales.
- **Severity**: serious
- **Timestamp**: [27:37](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1657)

### Generation is slow, taking roughly a minute per image compared to Flux or Z Image.
- **Severity**: heads_up
- **Timestamp**: [24:57](https://www.youtube.com/watch?v=OA4gchz1Zcs&t=1497)

## Where to go next

Explore advanced layout refinement by holding Alt to select underlying elements and using 'Grab Background' for iterative composition adjustments.

## Concepts surfaced

[[ideogram-4]] · [[comfy-ui]] · [[bounding-box-control]] · [[local-ai-generation]] · [[kj-nodes]] · [[prompt-adherence]]
