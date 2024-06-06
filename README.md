Hi, I'm Amy! I'm the News Photo Editor of Vol. 120 of The Duke Chronicle, and I'm also a freelance photographer in Durham, NC. My 2024-2025 bookings are open. 

Please contact me at amy.zhang@duke.edu to book! 

Here's some of my work!

document.addEventListener('DOMContentLoaded', async function() {
    // Fetch user's posts using Instagram Basic Display API
    const accessToken = 'YOUR_ACCESS_TOKEN';
    const userId = 'USER_ID'; // Amy's user ID
    const apiUrl = `https://graph.instagram.com/amydotjpeg/media?access_token=${accessToken}&fields=id,permalink`;

    try {
        const response = await fetch(apiUrl);
        const data = await response.json();

        // Iterate over each post and embed it
        data.data.forEach(post => {
            const postUrl = post.permalink;

            // Create a container div for each post
            const postContainer = document.createElement('div');
            postContainer.classList.add('instagram-post');
            document.body.appendChild(postContainer);

            // Load the Instagram post with the given URL
            instgrm.Embeds.process(postContainer, {
                url: postUrl
            });
        });
    } catch (error) {
        console.error('Error fetching user\'s posts:', error);
    }
});


