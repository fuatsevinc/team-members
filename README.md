# team-members
Team_members
# Editor Web Application

Develop a web application that can manage your favorite movies and sort.

## Requirements

This is an assignment to showcase your abilities as a frontend developer.

Please follow all checkbox in 4 sections below as much as possible. (Tick/Un-tick which you can/can't do)

### 1. Tech stack.

Its best to used our recommended stack as its our product tech stack.

- [ ] Use [ReactJS 16.8 above](https://reactjs.org/) or [NextJS](https://nextjs.org).

- [ ] Use [Typescript](https://www.typescriptlang.org/) as much as possible. (Optional)

### 2. Knowledge of frontend architecture

- [ ] Use **CSS** to develop a **mobile first** and responsive design for desktop if possible (Mobile screen designs will not provide in this assignment, you are free to imagine by yourself.)

- [ ] Use a pre-processor **LESS** or **SASS** or **SCSS** (Optional)

- [ ] Use react Component to break down the design into re-usable UI pieces.

- example via [Frontend Layout Sample](#frontend-layout-sample)

- [ ] Use [React Hooks](https://reactjs.org/docs/hooks-intro.html) to write code.

- [ ] Store the data on your browser Web Storage API (use localstorage to store data instead to calling API, backend is not nessary)

### 3. Ability to work with requirements

- [ ] Follow all checkbox in [User story & Design](#user-story--design) section.

- [ ] Follow the given design as close as possible ([design directory](/design))

### 4. Communication skills and Explanation of your work

- [ ] Write a concise and informative description on how u approach this assignment in [Description.md](/Description.md)

## User story & Design

**You can use already designed screens in** [Figma](https://www.figma.com/file/sIPco3Rb4Hgl2oQmk8yq5D/editor?node-id=9%3A30) or create your own design.
**You can use already provided data in** ([data directory](/data))

Make sure u stick on all the components to styleguide.

### Login Page

- [ ] As a user, I can login only with my email adress.
- [ ] If a user is not exist in user data could not able to access redirect to invalid login page.

### Access Denied Page

- [ ] As a user, I can go to lugath home page by clicking on home button.
- [ ] If a user is not exist in user data could not

## Editor Overview Page

- [ ] As a user, I can view all my translations which is grouped by language-pair and show progress related translation job.
- [ ] As a user, I can go to Editor Page by clicking on Use Lugath editor button.

## Editor Content Edit Page

- [ ] As a user, I can see all segments in the list.
- [ ] As a user, I can search or filter over segments in the list.
- [ ] As a user, I can change the target text of a segment.
- [ ] As a user, I **can not** change the source text of a segment.
- [ ] As a user, I can edit the target text by clicking a segment that becomes an _editable inline textbox_.
- [ ] As a user, I can able to edit the next segment when editing a segment is done.
- [ ] As a user, I can see the changes of a segment history listed under history tab.
- [ ] As a user, I can revert a segment to any version under the history tab.
- [ ] As a user, I can see an overall progress **grouped by segments I've edited** and showing the total change.

## Frontend Layout Sample

This is a sample. Please create layout and re-usable component as part of the assignment

```
# Editor
  <div className="bem_convention_class">
    <Header>
      <HeaderTop>
        <Breadcrumb>
        <UserMenu>
        ...
      </HeaderTop>
      <HeaderBottom>
        <EditorToolKit/>
        ...
      </HeaderBottom>
    </Header>
    <Main>
      <EditorLayout>
        <LayoutRight>
          <Top>
            <ContentEditor>
          </Top>
          <Bottom>
            <ContentTools>
          </Bottom>
        </LayoutRight>
        <LayoutLeft>
          <Top>
            <DependenciesEditor>
          </Top>
          <Bottom>
            <ContentStats>
          </Bottom>
        </LayoutLeft>
      </EditorLayout>
    </Main>
  </div>

