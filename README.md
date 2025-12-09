# KhlnaSoft Docs

> [!IMPORTANT]
> For support, please reach out to your account team or contact **[support@khulnasoft.com](mailto:support@khulnasoft.com)**.

Welcome to the **KhlnaSoft documentation repository**! We're excited to have you contribute.
Our docs are built with **Next.js**, **TailwindCSS**, and deployed on **Vercel**.
This guide will help you quickly set up your environment and start contributing.

---

## 🚀 Getting Started

Clone the repository:

```sh
git clone https://github.com/khulnasoft/docs.git docs
cd docs
```

### Prerequisites

Make sure your system uses the following versions:

* **Node.js:** `v20.8.1`
* **pnpm:** `8.13.1`

If you use **mise**, you can install the correct versions automatically:

```sh
mise install
```

### Install Dependencies

```sh
pnpm install
```

### Start the Development Server

```sh
pnpm dev
```

Visit: **[http://localhost:3000](http://localhost:3000)**

---

## ✍️ Contributing to KhlnaSoft Docs

### Option 1: (Easy) Edit Using GitHub

You can make quick edits directly from GitHub:

1. Navigate to the relevant `.mdx` file (see [Folder Structure](#folder-structure))
2. Click the **pencil icon**
3. Make your changes
4. Click **Commit changes…**
5. Add a commit message & description
6. Click **Propose changes**
7. Assign a reviewer via the gear icon

> **Note:** GitHub editing is ideal for text-only edits.
> For structural changes (React components, custom layouts, code blocks), use a local environment.

---

### Option 2: (Advanced) Local Development Workflow

Create a new branch:

```sh
git switch -c BRANCH_NAME_HERE
```

Make your changes locally and preview them using `pnpm dev`.

---

## 📂 Folder Structure

All documentation lives in the `/docs` directory.

Each product area (e.g., `cody`, `code_search`, `cli`) has its own folder.

To contribute:

* Navigate to the correct section
* Create a new `.mdx` file if you're adding a new page (e.g. `my-new-page.mdx`)

---

## 📝 Writing with MDX

We use **MDX**, which allows Markdown + React components.

Example:

```mdx
# Heading 1

This is an introductory paragraph.

## Heading 2

### Heading 3

Details for heading three.

This is a [demo link](https://khulnasoft.com/)

- Bullet 1
- Bullet 2
- Bullet 3
```

---

## 🧩 Using React Components

The docs include reusable components located in `src/components`.

Common components:

* `<QuickLinks>`
* `<ProductLinks>`
* `<LinkCards>`
* `<Callout>`

Example:

```mdx
<Callout type="note">Cody is currently in Beta for all users.</Callout>
```

These components help maintain consistent styling and layout across the docs.

---

## 🔗 Adding Internal Links

Use this format:

```md
[Link text](path-to-link)
```

Guidelines:

* **Do NOT include `/docs`** in links
* **Do NOT include `.mdx` extensions**

Examples:

```md
[Cody Quickstart](/cody/quickstart)

[Cody for VSCode installation](/cody/clients/install-vscode#verifying-the-installation)
```

---

## 👀 Previewing Changes

### Local Preview

Visit:

```
http://localhost:3000
```

The dev server hot-reloads as you edit.

### Vercel Preview Deployments

Every PR automatically gets a Vercel preview link.
Click **Visit Preview** in the deployment section of your PR.

---

## ✅ Submitting Your Contribution

Once you're ready:

1. Commit your changes
2. Open a PR

Thank you for contributing to **KhlnaSoft Docs**!
Your work helps us create a world-class documentation experience.