##Bluesky Style Analyzer

A web application that analyzes Bluesky posts and generates responses in Elon Musk's writing style using the Gemini AI model.

## Features

- Analyze any public Bluesky post using its URL
- Generate responses mimicking Elon Musk's communication style
- Clean, modern UI with a gradient design
- Real-time loading states and error handling
- Mobile-responsive layout

## Prerequisites

- Google Cloud Platform account for Gemini API access
- Bluesky account credentials
- Modern web browser with JavaScript enabled

## Setup

1. Clone this repository to your local machine

2. Create a `config.js` file in the root directory with your API configurations:
```javascript
const GEMINI_API_KEY = 'your-gemini-api-key';
```

3. Update the Bluesky credentials in the `getPostContent` function:
```javascript
const agent = {
    service: 'https://bsky.social',
    identifier: 'your-identifier',
    password: 'your-password'
};
```

4. Open `index.html` in a web browser or deploy to your preferred hosting service

## Usage

1. Navigate to the web application
2. Paste a Bluesky post URL in the input field (format: https://bsky.app/profile/...)
3. Click "Analyze & Generate"
4. View the original post and the AI-generated Elon Musk style response

## Technologies Used

- HTML5/CSS3
- JavaScript (Vanilla)
- Tailwind CSS for styling
- Google's Gemini AI API
- Bluesky Social API
- Web Animations API

## API Endpoints

The application uses two main APIs:

1. Gemini AI API
   - Endpoint: `https://generativelanguage.googleapis.com/v1beta/models/gemini-1.0-pro:generateContent`
   - Used for generating Elon Musk style responses

2. Bluesky Social API
   - Endpoint: `https://bsky.social/xrpc/com.atproto.repo.getRecord`
   - Used for fetching original post content

## Styling

The application features a custom design with:
- Gradient backgrounds
- Frosted glass effect cards
- Smooth animations
- Responsive layout
- Loading states with animations

## Error Handling

The application includes error handling for:
- Invalid URLs
- API failures
- Network issues
- Authentication errors

## Limitations

- Requires valid Bluesky post URLs
- Needs active internet connection
- API rate limits may apply
- Only works with public Bluesky posts

## Future Improvements

- Add user authentication
- Support for multiple AI models
- Batch processing of posts
- Save/export generated responses
- Additional writing style options
- Response history tracking

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.
