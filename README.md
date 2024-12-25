# Personal Projects API

This is a simple API that serves data related to various personal projects. The API fetches a list of projects and provides information such as project name, description, tools used, and more. It is designed to be used with a frontend application, where users can fetch and display projects dynamically.

## Features

- Fetch a list of projects with relevant details.
- Pagination support for better navigation through large lists of projects.
- Responsive and error-handling mechanisms for robust interaction.

## API Endpoints

### `GET /`
Fetches a list of projects. This endpoint returns the following project data:
- `name`: The name of the project.
- `image`: A URL to an image associated with the project.
- `description`: A brief description of the project.
- `tools`: The tools or technologies used in the project.
- `source`: A link to the source code or repository.
- `url` : Url of live demo of project.

**Example Response:**
```json
[
  {
    "_id": "1",
    "name": "Project 1",
    "image": "https://example.com/image.jpg",
    "description": "A brief description of the project.",
    "url" : "https://project-1.netlify.com",
    "tools": ["React", "Node.js", "MongoDB"],
    "source": "https://github.com/yourusername/project1"
  },
  {
    "_id": "2",
    "name": "Project 2",
    "image": "https://example.com/image2.jpg",
    "description": "Another project description.",
    "url" : "https://project-2.netlify.com",
    "tools": ["Vue", "Express", "MySQL"],
    "source": "https://github.com/yourusername/project2"
  }
]
