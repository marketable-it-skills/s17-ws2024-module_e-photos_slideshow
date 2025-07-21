# Test Project Outline – Module E – Photos Slideshow

## Competition time

4 hours

## Introduction

This project challenges students to create an interactive photo slideshow web application that demonstrates advanced frontend development skills. Students will build a comprehensive photo management and display system featuring drag-and-drop functionality, multiple animation themes, and various slideshow operating modes. The project emphasizes modern web technologies, user interface design, CSS animations, and interactive user experience principles suitable for real-world web application development.

## General Description of Project and Tasks

The project requires building a complete photo slideshow application with the following key components:

- **Photo Management**: Drag-and-drop photo loading, file input fallback, sample photo loading
- **Slideshow Modes**: Manual keyboard control, auto-playing with looping, random photo display
- **Visual Themes**: Six different animation themes (A-F) with CSS transitions and effects
- **User Interface**: Configuration panel, command bar with keyboard shortcuts, fullscreen mode
- **Technical Features**: Photo ordering, caption generation, responsive design, cross-browser compatibility

Students must demonstrate proficiency in HTML structure, advanced CSS animations, JavaScript event handling, Web APIs (File API, Fullscreen API), and creating polished user interfaces suitable for modern web applications.

## Requirements

The goal of the application is to provide users with a comprehensive photo slideshow tool that combines intuitive file management with visually appealing presentation options. Users must be able to load photos through multiple methods, organize them as needed, and display them using various animation themes and operating modes. The application should demonstrate modern web development practices while maintaining cross-browser compatibility and accessibility.

The slideshow tool should simulate real-world photo presentation applications, emphasizing user experience, visual design, and technical functionality. All features must work seamlessly together to create a cohesive and professional photo slideshow experience.

The application must be accessible at the URL pattern: `http://wsXX.worldskills.org/XX_module_e/` where XX represents the competitor number.

The following functionality must be implemented:

## Contents

- Date: 21.08.
  - Version: 1.
- Introduction
- Description of project and tasks
- Loading photos
- Configuration
- Themes
- Command bar
- Instructions to the Competitor
- Other

### Date: 21.08.

```
Version: 1.
```

**Introduction**

In this project, a client asks you to create a photo slideshow tool.

User is able to load external photos, or load sample photos into the slideshow. Then, photos appear, stay for
several seconds, and disappear, one by one. There may have transition and animation for appearing and
disappearing of photos, depending on the theme applied.

The project should be reachable at [http://wsXX.worldskills.org/XX_module_e/.](http://wsXX.worldskills.org/XX_module_e/.)

**Description of project and tasks**

There are different modes for the photo slideshow playing:

- Manual mode with left and right keyboard keypress.
- Auto-playing that photos keep coming in, and loop to the first photo after the last photo shows.
- Random playing the photos, which randomly a new photo shows after several seconds. In this mode, the
  slideshow runs forever and never ends.

The photo slideshow can also be turned into full screen browsing. The browser toolbar and windows task bar
are hidden after full-screen.

**Loading photos**

User can load photos by dragging the photo files into the drop area. Then these photos are displayed and played
according to the theme animation.

When the CSS is not available, or if CSS is disabled, user can still select the photo files via the file input. The
photos will then be loaded and listed into the web page. And no styles needed to apply.

**Captions**

The caption of the photos is defined by the filename. Please capitalize the remove slug of the filename. And the
caption doesn't contain a file extension.

For example, given a filename named "hello.jpg", the caption is Hello.

For example, the caption for "hello world.jpg" will be "Hello World".

For example, the caption for the "a-sample-photo.jpg" will be "A Sample Photo".

**Configuration**

There is a configuration panel. There are three configuration parts in the panel: operating mode, the active
theme switching, and the sorting of the photos.

**Switching operating**

In the panel, user can switch between 3 operating modes: manual control, auto-playing, random playing.

**Switching theme**

In the panel, user can switch between A to F theme.

**Ordering photos**

In this configuration panel, user can order the selected photos by drag and drop the photos.

```
Date: 21.08.
Version: 1.
```

**Themes**

The first 5 themes are pre-defined, they are Theme A, B, C, D, and E. Then you are going to create your own
Theme F.

**Theme A**

Theme A displays the photos and captions directly, without any effects.

**Theme B**

The active photo goes from left to right to the middle, then the photo goes from the middle to the right to leave
the screen.

For the caption, the caption element follows the left-to-right animation, but with a delay of 300ms to start the
animation.

Please find the theme-b-demo.mp4 from the media files for reference.

**Theme C**

The active photo goes from bottom to top to the middle, then the photo goes from middle to the top to leave
the screen.

For the caption, the caption is separated into words and each word animates up with a 300ms delay each.

Please find the theme-c-demo.mp4 from the media files for reference.

**Theme D**

The active photo slides in from the left to the middle of the screen. Then the photo stays in the middle. Next
photos slides in and to be placed on top of the active photos.

Each photo has a random slight rotation between -5 degree to 5 degree.

These photos should not take up all the screen space. They should be approximately 85% of the screen space.
This should create a feeling of stack of photos, because of the different rotation of the photos.

Each photo has a 3px of white border, with border radius 5px. And the bottom border looks thicker because of
the caption. For the caption, it should be at the bottom of the photos, with background color sharing the same
white color of the photo border.

Please find the theme-d-demo.mp4 from the media files for reference.

**Theme E**

The active photo is displayed in the middle of the screen. Then there is a door opening effect for the current
photo. The active photo is split into two halves, left half and right half part of the photo. Then the left and right
half of the photo rotate into the screen with 3D perspective to create a door opening effect.

The next photo appears from the back to the front and become active after the current photo disappear.

In this theme, no photo captions are displayed.

Please find the theme-e-demo.mp4 from the media files for reference.

**Theme F**

Please create a new them named "Theme F". You can define your photo sliding transition and captions
animation. Please make sure they are appealing.

**Sample photos**

There is an option to load sample photos instead of dragging in custom photos.

```
Date: 21.08.
Version: 1.
```

**Command bar**

User can show command bar by pressing CTRL+K or "/". And user can return to normal from command bar
dialog by pressing ESC key.

The command bar is usually placed in the middle of the screen. When the command bar is activated, the other
part of the web page is dimmed.

When the command bar is activated, the other part of the web page is dimmed.

During command bar is presented, different options are displayed under the command bar input.

User can select different options by pressing keyboard up and down.

The selected option should be highlighted for user to know.

When user press ENTER key, the selected option is executed as the command.

There are following commands in the command bar:

- Change to manual control mode
- Change to auto-playing mode
- Change to random playing mode
- Switch to theme A
- Switch to theme B
- Switch to theme C
- Switch to theme D
- Switch to theme E
- Switch to theme F

**Instructions to the Competitor**

CSS for the themes should be well organized into different files for easy maintenance and considered separate
of concern.

**Other**

The project should be reachable at [http://wsXX.worldskills.org/XX_module_e/](http://wsXX.worldskills.org/XX_module_e/) URL.
If you have put your work in sub-folders, or in other port such as :3000, you may redirect to the destination from
the /XX_module_e/ path.

You may provide a README file for executing guide if necessary.

## Assessment

The project will be assessed using comprehensive evaluation methods to ensure both technical implementation and user experience meet professional standards:

**Technical Assessment:**
- Functionality testing of all slideshow modes and theme implementations
- Cross-browser testing in Firefox Developer Edition and Google Chrome
- Code quality assessment for HTML structure, CSS organization, and JavaScript implementation
- Web API integration verification (File API, Fullscreen API)
- Performance evaluation of animations and large image handling

**User Experience Evaluation:**
- Interface usability and intuitive navigation assessment
- Visual design quality and animation smoothness evaluation
- Drag-and-drop functionality and user feedback systems
- Keyboard navigation and accessibility compliance testing
- Configuration panel and command bar usability verification

**Assessment Tools:**
- Firefox Developer Edition and Google Chrome web browsers for primary testing
- Browser developer tools for performance analysis and debugging verification
- Manual testing of all user workflows and interaction patterns
- Code review using web development best practices and standards
- Responsive design testing across different screen sizes and devices

## Mark distribution

| WSOS SECTION | Description                            | Points |
|--------------|----------------------------------------|--------|
| 1            | Work organization and self-management  | 0      |
| 2            | Communication and interpersonal skills | 0      |
| 3            | Design Implementation                  | 8.5    |
| 4            | Front-End Development                  | 5.5    |
| 5            | Back-End Development                   | 0      |
| **Total**    |                                        | **14** |
