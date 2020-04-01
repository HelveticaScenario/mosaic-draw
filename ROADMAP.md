# MVP

- user logs in
- user clicks the "draw" button
- server finds an active canvas with free blocks and sends its current state
- client subscribes to canvas changes
- server allocates next free block to user
- user is given some time limit to draw in their 5x5 block
- user submits their block to the server
- users block is added to the canvas in db
- every active user gets the new block pushed to them
- if canvas still has free blocks, the next free block is allocated to the user
- rinse and repeat until all blocks are allocated or completed
- if user abandons the canvas, their block is freed and available for allocation
  to the next user
- if the user clicks draw and there are no active canvases with free blocks, a
  new canvas is created.

# 0.1.0

- [ ] canvas and block tables
- [ ] canvas viewer
- [ ] block editor
- [ ] user history page
